# Backup your emacs configs so you can hacking anywhere

As a programmer and a emacs hacker, you may want to hacking in a consistent emacs
environment. When craft a useful .el config when working at one laptop, you may
want to share it to another computer at home(or at what so ever!). You can first
upload your configs to some cloud driver(such as google cloud storage...), then
download your configs on other computer and use it. It costs your money and waste
your time. Why not use github, your best micro:) cloud driver...

## 1. Presets
+ Install the latest emacs on your computer
+ Your computer can connect to the internet
+ Have *curl* as a component of your system(if not, just install it)
+ Your system can execute bash script

As a hacker, you deserve to use unix/linux as your develop os. :)) But this tutorial
can be used under windows too, but i personally advise you leave it for a better 
life.

## 2. Orchestrate your emacs config directory
When you start emacs, it will first load config files. If you have a .emacs file
under your home directory, it will first load that file. But i highly recommend 
you use the *init.el* file under *~/.emacs.d*. The following is the tree of my
configs:

![config directory](./graph/configdir.png)
