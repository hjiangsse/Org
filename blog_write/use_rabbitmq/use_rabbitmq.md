
# Table of Contents

1.  [basic usage:](#org0b69a30)
    1.  [send/receive pattern:](#org0aeff73)
        1.  [send a message to a queue:](#org9d3ad2c)
        2.  [receive a message from a queue:](#org0f873ef)
    2.  [working queue pattern:](#org606627c)
    3.  [deal with message acknowledgment:](#org4483c61)
    4.  [RabbitMQ message durability:](#org0d824a7)
        1.  [publisher and subcriber queue durability not match](#org9a48540)
        2.  [publisher use a durable queue, but the messages it send not persistent](#orga1e2e9e)
        3.  [messages fair dispatch](#org54892c4)
    5.  [publish/subcriber pattern](#orgaf9dbd4)
        1.  [declear an exchange](#org547a14f)
        2.  [use temporary queues](#org04ecab4)
        3.  [do pub/sub](#org2b74b80)
    6.  [routing(receiving messages selectively)](#org79eb90c)
    7.  [topics(receiving messages based on a pattern)](#org55ca525)
    8.  [RPC (request/reply pattern)](#org2747354)


<a id="org0b69a30"></a>

# basic usage:


<a id="org0aeff73"></a>

## send/receive pattern:


<a id="org9d3ad2c"></a>

### send a message to a queue:

    package main
    
    import (
    	"log"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel, which encapsulates most APIs get things done
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	//declare a queue for us to send to,
    	//then publish messages to this queue
    	//queue has a name, just like "subject" in nats
    	//or "topic" in nsqd
    	q, err := ch.QueueDeclare(
    		"hello", //name
    		false,   //durale
    		false,   //delete when unused
    		false,   //exclusive
    		false,   //no wait
    		nil,     //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	msgBody := "Hello RabbitMq"
    	err = ch.Publish(
    		"",     //exchange
    		q.Name, //routine key
    		false,  //mandatory
    		false,  //immediate
    		amqp.Publishing{
    			ContentType: "text/plain",
    			Body:        []byte(msgBody),
    		})
    	failOnError(err, "Failed to publish a message")
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

in the previous code, we send a message to a queue, which name is "hello";


<a id="org0f873ef"></a>

### receive a message from a queue:

    package main
    
    import (
    	"log"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	//declare a queue for us to send to,
    	//then publish messages to this queue
    	q, err := ch.QueueDeclare(
    		"hello", //name
    		false,   //durale
    		false,   //delete when unused
    		false,   //exclusive
    		false,   //no wait
    		nil,     //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	msgs, err := ch.Consume(
    		q.Name,
    		"",
    		true,  //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			log.Printf("Recived a message: %s\n", d.Body)
    		}
    	}()
    
    	log.Printf(" [*]Waiting for message, To exit press Ctrl+C")
    	<-forever
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

in the previous code, we receive a message from a queue, which name is "hello";


<a id="org606627c"></a>

## working queue pattern:

working queue is used to distribute tasks among multiple workers;

    package main
    
    import (
    	"log"
    	"os"
    	"strings"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	//declare a queue for us to send to,
    	//then publish messages to this queue
    	q, err := ch.QueueDeclare(
    		"hello-tasks", //name
    		false,         //durale
    		false,         //delete when unused
    		false,         //exclusive
    		false,         //no wait
    		nil,           //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	msgBody := bodyFrom(os.Args)
    	err = ch.Publish(
    		"",     //exchange
    		q.Name, //routine key
    		false,  //mandatory
    		false,  //immediate
    		amqp.Publishing{
    			DeliveryMode: amqp.Persistent,
    			ContentType:  "text/plain",
    			Body:         []byte(msgBody),
    		})
    	failOnError(err, "Failed to publish a message")
    }
    
    func bodyFrom(args []string) string {
    	var s string
    	if (len(args) < 2) || os.Args[1] == "" {
    		s = "hello..."
    	} else {
    		s = strings.Join(args[1:], " ")
    	}
    	return s
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

in the code, we simulate a task by "dots" in the message, example: hello&#x2026;
is a task need to excute 3 seconds;

    go run new_tasks.go hello....

refactor the receiver code:

    package main
    
    import (
    	"bytes"
    	"log"
    	"time"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	//declare a queue for us to send to,
    	//then publish messages to this queue
    	q, err := ch.QueueDeclare(
    		"hello-tasks", //name
    		false,         //durale
    		false,         //delete when unused
    		false,         //exclusive
    		false,         //no wait
    		nil,           //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	msgs, err := ch.Consume(
    		q.Name,
    		"",
    		true,  //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			log.Printf("Recived a message: %s\n", d.Body)
    			dotCnt := bytes.Count(d.Body, []byte("."))
    			log.Printf("This worker will sleep %d seconds.\n", dotCnt)
    			t := time.Duration(dotCnt)
    			time.Sleep(t * time.Second)
    			log.Println("Done")
    		}
    	}()
    
    	log.Printf(" [*]Waiting for message, To exit press Ctrl+C")
    	<-forever
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

now let's see how the messages in queue dispatched:
open three terminal, two for workers and one for the task-generator:

go run worker.go

go run worker.go

![img](./graph/new_tasks.png)
let's see what happen to the shell 1 and shell 2:
![img](./graph/shell1.png)
shell 1 receive message 1,3,5
![img](./graph/shell2.png)
shell 2 receive message 2,4
every consumer will get the same number of messages;


<a id="org4483c61"></a>

## deal with message acknowledgment:

what will happen when one worker crash down? if 
not all the messages is been processed? RabbitMq can use
"acks" to make sure no message lost even if the workers
occasionally die.

first let's see what happen when "acks" not used;
in the "working queue pattern" we send the 6th message:

    go run new_tasks.go sixth Message..........

shell 2:
[the 6th message shell 2](graph/shell2-kill.png)
when enter "Ctrl+C" in shell 2, nothing happen in shell 1;
so, we can deduce that 6th message is losting forever;

we change code in "worker.go":

    msgs, err := ch.Consume(
    		q.Name,
    		"",
    		//true,  //auto ack
    		false, //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			log.Printf("Recived a message: %s\n", d.Body)
    			dotCnt := bytes.Count(d.Body, []byte("."))
    			log.Printf("This worker will sleep %d seconds.\n", dotCnt)
    			t := time.Duration(dotCnt)
    			time.Sleep(t * time.Second)
    			log.Println("Done")
    			d.Ack(false)
    		}
    	}()

    we set "autoack" in the consumer to false; means that when the worker
finish task, it will not send a ack automaticlly; so this require us to manually
send a "ack" &#x2013; "d.Ack(false)"; let's see how this will affect message dilivery:
    [send five tasks to rebbitMq](graph/ack_send.png)

the fifth message will be delivered to the shell 1 according the round robin method.
then we manually kill the session in shell 1. this is what we get:

[manually kill shell 1 session when recv the 5th message](graph/ack_shell1.png)

after the worker in shell 1 is killed, the 5th message will redeliver to worker in shell 2:

[the 5th message redeliver to shell 2](graph/ack_shell2.png)


<a id="org0d824a7"></a>

## RabbitMQ message durability:

when rabbitmq quite or crash, the queues and messages in these queues will losted!
we need to mark both the queue and messages as durable.
(the publishers and subscribers both declear them as durable)


<a id="org9a48540"></a>

### publisher and subcriber queue durability not match

if the publisher declear the queue as durable:

    //declare a queue for us to send to,
    //then publish messages to this queue
    q, err := ch.QueueDeclare(
    	"hello-tasks-dur", //name
    	true,  //durable
    	false, //delete when unused
    	false, //exclusive
    	false, //no wait
    	nil,   //arguments
    )

but the subcriber not declear the queue as durable:

    //declare a queue for us to send to,
    //then publish messages to this queue
    q, err := ch.QueueDeclare(
    	"hello-tasks-dur", //name
    	false,             //durale
    	false,             //delete when unused
    	false,             //exclusive
    	false,             //no wait
    	nil,               //arguments
    )

when we run the worker: go run worker.go, we get an error:
[queue durablity not match error](graph/durable_no_match.png)

after change subscriber's queue declearation:

    q, err := ch.QueueDeclare(
    	"hello-tasks-dur", //name
    	true,              //durale
    	false,             //delete when unused
    	false,             //exclusive
    	false,             //no wait
    	nil,               //arguments
    )

run the worker again:
[the durability of publisher and subcriber matches](graph/durable_match.png)


<a id="orga1e2e9e"></a>

### publisher use a durable queue, but the messages it send not persistent

in the publisher, when we send a message:

    err = ch.Publish(
    		"",     //exchange
    		q.Name, //routine key
    		false,  //mandatory
    		false,  //immediate
    		amqp.Publishing{
    			//DeliveryMode: amqp.Persistent,
    			ContentType: "text/plain",
    			Body:        []byte(msgBody),
    		})

we publish two message to server:

[publish two no-durable messages to rabbitmq-server](graph/publish_two_nodure_messages.png)

then use rabbitmqctrl tool inspect the server:

[rabbitmq queues inspection](graph/inspect_queues_1.png)

but after that we restart rabbitmq-server:
**sudo serveice restart rabbitmq-server**
then inspect queues again:

[inspect the queues when the sended messages are not durable](graph/inspect_qqueue_2.png)

so we can get a conclusion: In order to get "message durability", we must provide 
the follow guarantee:

1.  a durable queue;
2.  the messages which in this queue is persistent;


<a id="org54892c4"></a>

### messages fair dispatch

in the previous examples, rabbitmq-server dispatch messages using a round robin method;
it do not look the number of unacknowledged messages for a consumer. 

    err = ch.Qos(1, //prefetch count
    			 0, //prefetch size
    			 false)
    failOnError(err, "Failed to set Qos")

prefetch count set to 1, agree that is server not receive a ack from client, it will not
dispatch the next message to this client.


<a id="orgaf9dbd4"></a>

## publish/subcriber pattern


<a id="org547a14f"></a>

### declear an exchange

deliver a message to multiple consumers, the core idea in the messaging model in RabbitMQ:

[the core messaging model in rabbitmq](graph/rabbit_exchange_model.png)

the producer send its message to an "Exchange", the exchange deliver this message to queues it
knows; so the producer have no knowledge about any queue.

now we can publish message to a named exchange:

    package main
    
    import (
    	"log"
    	"os"
    	"strings"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672/")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	err = ch.ExchangeDeclare(
    		"logs",   // nane
    		"fanout", // type
    		true,     // durable
    		false,    // auto-deleted
    		false,    // internal
    		false,    // no-wait
    		nil,      // arguments
    	)
    	failOnError(err, "Failed to declear an exchange")
    
    	msgBody := bodyFrom(os.Args)
    	err = ch.Publish(
    		"logs", //exchange
    		"",     //routine key
    		false,  //mandatory
    		false,  //immediate
    		amqp.Publishing{
    			DeliveryMode: amqp.Persistent,
    			ContentType:  "text/plain",
    			Body:         []byte(msgBody),
    		})
    	failOnError(err, "Failed to publish a message")
    }
    
    func bodyFrom(args []string) string {
    	var s string
    	if (len(args) < 2) || os.Args[1] == "" {
    		s = "hello..."
    	} else {
    		s = strings.Join(args[1:], " ")
    	}
    	return s
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

when we run the code, then use rabbitmqctrl to inspect exchange messages:

[list all the exchages after declear an exchange](graph/list-exchanges.png)

we can see our exchange which name is "logs" and type is "fanout"; in the code
snippet, the publisher just declear a exchange and send message to this exchange;


<a id="org04ecab4"></a>

### use temporary queues

subscriber need the follow step:
declear exchange(same as the publisher)

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<tbody>
<tr>
</tr>
</tbody>

<tbody>
<tr>
</tr>
</tbody>
</table>

		v
declear temp queue 

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<tbody>
<tr>
</tr>
</tbody>

<tbody>
<tr>
</tr>
</tbody>
</table>

		v
bind temp queue to the exchange 

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<tbody>
<tr>
</tr>
</tbody>

<tbody>
<tr>
</tr>
</tbody>
</table>

		v
waiting message on the queue:

    package main
    
    import (
    	"log"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	err = ch.ExchangeDeclare(
    		"logs",   // nane
    		"fanout", // type
    		true,     // durable
    		false,    // auto-deleted
    		false,    // internal
    		false,    // no-wait
    		nil,      // arguments
    	)
    	failOnError(err, "Failed to declear an exchange")
    
    	q, err := ch.QueueDeclare(
    		"",    //empty name
    		false, //durale
    		false, //delete when unused
    		true,  //exclusive
    		false, //no wait
    		nil,   //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	//bind queue to a exchange
    	err = ch.QueueBind(
    		q.Name,
    		"",
    		"logs",
    		false,
    		nil,
    	)
    	failOnError(err, "Failed to bind the queue to exchange")
    
    	msgs, err := ch.Consume(
    		q.Name,
    		"",
    		true,  //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			log.Printf("Recived a message: %s\n", d.Body)
    		}
    	}()
    
    	log.Printf(" [*]Waiting for message, To exit press Ctrl+C")
    	<-forever
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }


<a id="org2b74b80"></a>

### do pub/sub

[run a subscriber and redirect the messages to file](graph/subscribe_run.png)

[run a subscriber and redirect the messages to console](graph/subscribe_run_console.png)  

then publish three message to the "logs" exchange on server:
[publish three messages to "logs" exchange](graph/publish_to_exchange.png)

then we look at the two subscribers:
[subcribe 1 messages receive](graph/subscriber_1.png)

[subscriber 2 recieve messages](graph/subscriber_2.png)

use rabbitmqctrl check the queue binding information:
[list queue bindings after two subscriber running](graph/queue_bindings.png)
two rand-name queue is binding the "logs" exchange.


<a id="org79eb90c"></a>

## routing(receiving messages selectively)

In some sences, one subscriber only want to receive a subset messages from 
the exchange.we can use the "routing<sub>key</sub>" in queue binding, a subscriber 
only intrest the message with such "routing<sub>key</sub>".

We can do an experiment, publisher generate a ball in random color every second;
then send the ball to exchange; one subscriber only interest the red balls, so it
bind the queue use "red" as the "routing<sub>key</sub>"; another subscriber interest green
and blue balls, so it bind the queue use "green" and "blue" as the "routing<sub>key</sub>".

publisher.go:

    package main
    
    import (
    	"log"
    	"math/rand"
    	"os"
    	"strings"
    	"time"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	routineKeys := []string{"red", "green", "blue"}
    
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672/")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	err = ch.ExchangeDeclare(
    		"balls",  // name
    		"direct", // this is a direct exchange
    		true,     // durable
    		false,    // auto-deleted
    		false,    // internal
    		false,    // no-wait
    		nil,      // arguments
    	)
    	failOnError(err, "Failed to declear an exchange")
    
    	msgBody := bodyFrom(os.Args)
    	for {
    		keyIdx := rand.Intn(3)
    
    		err = ch.Publish(
    			"balls",             //exchange
    			routineKeys[keyIdx], //routine key
    			false,               //mandatory
    			false,               //immediate
    			amqp.Publishing{
    				DeliveryMode: amqp.Persistent,
    				ContentType:  "text/plain",
    				Body:         []byte(msgBody + "[" + routineKeys[keyIdx] + "]"),
    			})
    		failOnError(err, "Failed to publish a message")
    
    		time.Sleep(time.Second)
    	}
    }
    
    func bodyFrom(args []string) string {
    	var s string
    	if (len(args) < 2) || os.Args[1] == "" {
    		s = "hello..."
    	} else {
    		s = strings.Join(args[1:], " ")
    	}
    	return s
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

publisher send balls to an exchange which name is "balls", each publish
use a random routine key;

subscribe.go:

    package main
    
    import (
    	"log"
    	"os"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	err = ch.ExchangeDeclare(
    		"balls",  // nane
    		"direct", // type
    		true,     // durable
    		false,    // auto-deleted
    		false,    // internal
    		false,    // no-wait
    		nil,      // arguments
    	)
    	failOnError(err, "Failed to declear an exchange")
    
    	q, err := ch.QueueDeclare(
    		"",    //empty name
    		false, //durale
    		false, //delete when unused
    		true,  //exclusive
    		false, //no wait
    		nil,   //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	//bind queue to a exchange
    	for _, routinekey := range os.Args[1:] {
    		log.Printf("Binding queue %s to exchange %s with routing key %s",
    			q.Name, "balls", routinekey)
    
    		err = ch.QueueBind(
    			q.Name,
    			routinekey,
    			"balls",
    			false,
    			nil,
    		)
    		failOnError(err, "Failed to bind the queue to exchange")
    	}
    
    	msgs, err := ch.Consume(
    		q.Name,
    		"",
    		true,  //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			log.Printf("Recived a message: %s\n", d.Body)
    		}
    	}()
    
    	log.Printf(" [*]Waiting for message, To exit press Ctrl+C")
    	<-forever
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

subcriber receive messages selectively. the subcriber which only receive red ball:

[subsciber which only recieve red ball](graph/sub_red.png)

the subscriber which recieve green and blue ball:

[subcriber only recieve blue and green balls](graph/sub_blue_green.png)    

this messages routine setup:

[message routine setup](graph/routine_setup.png)


<a id="org55ca525"></a>

## topics(receiving messages based on a pattern)

if we want some more flexibility when receive messages on server, we can
try a new kind of exchange: topic.

topic rule: the routing<sub>key</sub> of topic must be a list of words, delimited by
dots, two important special cases for binding keys:

    * (star) can substitute for exactly one word.
    # (hash) can substitute for zero or more words.

now we do an experiment, we create a topic exchange by publisher; one subcriber
bind a queue with the topic exchage using "**.orange.**" as routine-key; another
subscriber use two routine-keys: "**.**.rabbit" and "lazy.#", following is the setup:

[animals topic setup](graph/topic_setup.png)
Fig.1 topic exchange routine setup

topic<sub>pub.go</sub>

    package main
    
    import (
    	"log"
    	"math/rand"
    	"os"
    	"strings"
    	"time"
    
    	"github.com/streadway/amqp"
    )
    
    var characters = []string{"strive", "mediocrity", "lazy"}
    var colors = []string{"red", "green", "orange"}
    var animals = []string{"rabbit", "tiger", "duck"}
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672/")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	err = ch.ExchangeDeclare(
    		"animal-checking", // nane
    		"topic",           // type
    		true,              // durable
    		false,             // auto-deleted
    		false,             // internal
    		false,             // no-wait
    		nil,               // arguments
    	)
    	failOnError(err, "Failed to declear an exchange")
    
    	msgBody := bodyFrom(os.Args)
    	for {
    		rtkey := genRouteKey()
    
    		err = ch.Publish(
    			"animal-checking", //exchange
    			rtkey,             //routine key
    			false,             //mandatory
    			false,             //immediate
    			amqp.Publishing{
    				DeliveryMode: amqp.Persistent,
    				ContentType:  "text/plain",
    				Body:         []byte(msgBody + "[" + rtkey + "]"),
    			})
    		failOnError(err, "Failed to publish a message")
    
    		time.Sleep(time.Second)
    	}
    }
    
    func genRouteKey() string {
    	chaIdx, corIdx, aniIdx := rand.Intn(3), rand.Intn(3), rand.Intn(3)
    	return characters[chaIdx] + "." + colors[corIdx] + "." + animals[aniIdx]
    }
    
    func bodyFrom(args []string) string {
    	var s string
    	if (len(args) < 2) || os.Args[1] == "" {
    		s = "hello..."
    	} else {
    		s = strings.Join(args[1:], " ")
    	}
    	return s
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

in the code, we publish message use a random generate routine-key;

topic<sub>sub.go</sub>

    package main
    
    import (
    	"log"
    	"os"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	err = ch.ExchangeDeclare(
    		"animal-checking", // nane
    		"topic",           // type
    		true,              // durable
    		false,             // auto-deleted
    		false,             // internal
    		false,             // no-wait
    		nil,               // arguments
    	)
    	failOnError(err, "Failed to declear an exchange")
    
    	q, err := ch.QueueDeclare(
    		"",    //empty name
    		false, //durale
    		false, //delete when unused
    		true,  //exclusive
    		false, //no wait
    		nil,   //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	if len(os.Args) < 2 {
    		log.Printf("Usage: %s [binding_key]...", os.Args[0])
    		os.Exit(0)
    	}
    
    	//bind queue to a exchange
    	for _, routinekey := range os.Args[1:] {
    		log.Printf("Binding queue %s to exchange %s with routing key %s",
    			q.Name, "animal-checking", routinekey)
    
    		err = ch.QueueBind(
    			q.Name,
    			routinekey,
    			"balls",
    			false,
    			nil,
    		)
    		failOnError(err, "Failed to bind the queue to exchange")
    	}
    
    	msgs, err := ch.Consume(
    		q.Name,
    		"",
    		true,  //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			log.Printf("Recived a message: %s\n", d.Body)
    		}
    	}()
    
    	log.Printf(" [*]Waiting for message, To exit press Ctrl+C")
    	<-forever
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

in the code, we subcribe message using command line arguments as routine-key;

\#shell 1
$go run topic<sub>sub.go</sub> **.orange.**

[wanting messages which routine-key is **.orange.**](graph/topic_sub_start_1.png)

\#shell 2
$go run topic<sub>sub.go</sub> **.**.rabbit lazy.#

[want messages which routine-key is **.**.rabbit or lazy.#](graph/topic_sub_start_2.png)

\#shell 3
$go run topic<sub>pub.go</sub> some animals comming!

shell 1 only receive **orange** animal:
[shell1 only receive orange animals](graph/shell_1_orange.png)

shell 2 recive all lazy animals and all kinds of rabbit, what a nightmare!!
[shell2 lazy and rabbit](graph/shell_1_lzay.png)


<a id="org2747354"></a>

## RPC (request/reply pattern)

want run a function on a remote computer and wait for the result.

a RPC server is waiting on a rpc<sub>queue</sub>, RPC client publish request
on the rpc<sub>queue</sub>; a RPC setup is like this:

[rpc<sub>setup</sub>](graph/rpc_setup.png)

rpc<sub>server.go</sub>

    package main
    
    import (
    	"log"
    	"strconv"
    
    	"github.com/streadway/amqp"
    )
    
    func main() {
    	//dial rabbitmq server
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672")
    	failOnError(err, "Failed to connect to RabbitMq")
    	defer conn.Close()
    
    	//create a channel
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to create channel")
    	defer ch.Close()
    
    	q, err := ch.QueueDeclare(
    		"rpc_queue", //empty name
    		false,       //durale
    		false,       //delete when unused
    		false,       //exclusive
    		false,       //no wait
    		nil,         //arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	err = ch.Qos(
    		1, //prefetch count
    		0, //prefetch size
    		false,
    	)
    
    	msgs, err := ch.Consume(
    		q.Name,
    		"",
    		false, //auto ack
    		false, //exclusive
    		false, //no-local
    		false, //no-wait
    		nil,   //args
    	)
    	failOnError(err, "Can not register a consumer")
    
    	forever := make(chan bool)
    
    	go func() {
    		for d := range msgs {
    			//log.Printf("Recived a message: %s\n", d.Body)
    			n, err := strconv.Atoi(string(d.Body))
    			failOnError(err, "Failed to convert body to integer")
    
    			log.Printf(" [.] fib(%d)", n)
    			response := fib(n)
    
    			err = ch.Publish(
    				"",        //use the default exchange
    				d.ReplyTo, //routing key
    				false,
    				false,
    				amqp.Publishing{
    					ContentType:   "text/plain",
    					CorrelationId: d.CorrelationId,
    					Body:          []byte(strconv.Itoa(response)),
    				},
    			)
    			failOnError(err, "Failed to publish a message")
    
    			d.Ack(false)
    		}
    	}()
    
    	log.Printf(" [*]Waiting for message, To exit press Ctrl+C")
    	<-forever
    }
    
    func fib(n int) int {
    	if n == 0 {
    		return 0
    	} else if n == 1 {
    		return 1
    	} else {
    		return fib(n-1) + fib(n-2)
    	}
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

rpc<sub>client.go</sub>

    	package main
    
    import (
    	"log"
    	"math/rand"
    	"os"
    	"strconv"
    	"strings"
    	"time"
    
    	"github.com/streadway/amqp"
    )
    
    func randomString(l int) string {
    	bytes := make([]byte, l)
    	for i := 0; i < l; i++ {
    		bytes[i] = byte(randInt(65, 90))
    	}
    	return string(bytes)
    }
    
    func randInt(min int, max int) int {
    	return min + rand.Intn(max-min)
    }
    
    func fibonacciRPC(n int) (res int, err error) {
    	conn, err := amqp.Dial("amqp://guest:guest@localhost:5672/")
    	failOnError(err, "Failed to connect to RabbitMQ")
    	defer conn.Close()
    
    	ch, err := conn.Channel()
    	failOnError(err, "Failed to open a channel")
    	defer ch.Close()
    
    	q, err := ch.QueueDeclare(
    		"",    // name
    		false, // durable
    		false, // delete when unused
    		true,  // exclusive
    		false, // noWait
    		nil,   // arguments
    	)
    	failOnError(err, "Failed to declare a queue")
    
    	msgs, err := ch.Consume(
    		q.Name, // queue
    		"",     // consumer
    		true,   // auto-ack
    		false,  // exclusive
    		false,  // no-local
    		false,  // no-wait
    		nil,    // args
    	)
    	failOnError(err, "Failed to register a consumer")
    
    	corrId := randomString(32)
    
    	err = ch.Publish(
    		"",          // exchange
    		"rpc_queue", // routing key
    		false,       // mandatory
    		false,       // immediate
    		amqp.Publishing{
    			ContentType:   "text/plain",
    			CorrelationId: corrId,
    			ReplyTo:       q.Name,
    			Body:          []byte(strconv.Itoa(n)),
    		})
    	failOnError(err, "Failed to publish a message")
    
    	for d := range msgs {
    		if corrId == d.CorrelationId {
    			res, err = strconv.Atoi(string(d.Body))
    			failOnError(err, "Failed to convert body to integer")
    			break
    		}
    	}
    
    	return
    }
    
    func main() {
    	rand.Seed(time.Now().UTC().UnixNano())
    
    	n := bodyFrom(os.Args)
    
    	log.Printf(" [x] Requesting fib(%d)", n)
    	res, err := fibonacciRPC(n)
    	failOnError(err, "Failed to handle RPC request")
    
    	log.Printf(" [.] Got %d", res)
    }
    
    func bodyFrom(args []string) int {
    	var s string
    	if (len(args) < 2) || os.Args[1] == "" {
    		s = "30"
    	} else {
    		s = strings.Join(args[1:], " ")
    	}
    	n, err := strconv.Atoi(s)
    	failOnError(err, "Failed to convert arg to integer")
    	return n
    }
    
    func failOnError(err error, msg string) {
    	if err != nil {
    		log.Fatalf("%s: %s", msg, err)
    	}
    }

