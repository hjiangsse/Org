





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
  <link rel="dns-prefetch" href="https://github.githubassets.com">
  <link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



  <link crossorigin="anonymous" media="all" integrity="sha512-UDS3MR1FfvqHmqZAs2MWSDCWPwLemVRLqCwld4/zfwH0vhv7I6RYmDnMnNAVQKP1YYvqnccOCH4iOhFaUUyrjw==" rel="stylesheet" href="https://github.githubassets.com/assets/frameworks-2e9090135c22aad5f56c2f72dcba7880.css" />
  <link crossorigin="anonymous" media="all" integrity="sha512-l4JpykYR1c86XfE0TExTqRFbnoD7WA39FhTTEgPt22zLFiepYq+L+3XUGBZoGsnBv15oKHTomwpEAUrCbmoRqw==" rel="stylesheet" href="https://github.githubassets.com/assets/site-2f0f446a127a5a480dfb139991acd1cd.css" />
    <link crossorigin="anonymous" media="all" integrity="sha512-D8GUhgLn0Pm94+eZHS2+GVyUSkcIQCn86Is/aPo/SqDdh84zzgsUc3pYlfSvK7YJvxqihMWsJET2Tsc6QOD5Ow==" rel="stylesheet" href="https://github.githubassets.com/assets/github-e0bb7eeb3d3f55bf57453459bf0da4e8.css" />
    
    
    
    

  <meta name="viewport" content="width=device-width">
  
  <title>golang-cheat-sheet/README.md at master · a8m/golang-cheat-sheet · GitHub</title>
    <meta name="description" content="An overview of Go syntax and features. Contribute to a8m/golang-cheat-sheet development by creating an account on GitHub.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    <meta name="twitter:image:src" content="https://avatars1.githubusercontent.com/u/7413593?s=400&amp;v=4" /><meta name="twitter:site" content="@github" /><meta name="twitter:card" content="summary" /><meta name="twitter:title" content="a8m/golang-cheat-sheet" /><meta name="twitter:description" content="An overview of Go syntax and features. Contribute to a8m/golang-cheat-sheet development by creating an account on GitHub." />
    <meta property="og:image" content="https://avatars1.githubusercontent.com/u/7413593?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="a8m/golang-cheat-sheet" /><meta property="og:url" content="https://github.com/a8m/golang-cheat-sheet" /><meta property="og:description" content="An overview of Go syntax and features. Contribute to a8m/golang-cheat-sheet development by creating an account on GitHub." />

  <link rel="assets" href="https://github.githubassets.com/">
  
  <meta name="pjax-timeout" content="1000">
  
  <meta name="request-id" content="A8AA:0B56:311D8D:450C23:5D6631B0" data-pjax-transient>


  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

      <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

  <meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="A8AA:0B56:311D8D:450C23:5D6631B0" /><meta name="octolytics-dimension-region_edge" content="ap-southeast-1" /><meta name="octolytics-dimension-region_render" content="iad" /><meta name="octolytics-dimension-ga_id" content="" class="js-octo-ga-id" /><meta name="octolytics-dimension-visitor_id" content="6106028918935269808" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



    <meta name="google-analytics" content="UA-3769691-2">


<meta class="js-ga-set" name="dimension1" content="Logged Out">



  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="NDMwMzc4NmQ3ZjEyZmJiYTNmZTNmM2NjNGQyMmJjZmIxZjkxZDBjZTMzMjEwODRiNzMzOTQyYjc0Y2ZjNmRhMXx7InJlbW90ZV9hZGRyZXNzIjoiNjEuMTI5LjEwMy44NyIsInJlcXVlc3RfaWQiOiJBOEFBOjBCNTY6MzExRDhEOjQ1MEMyMzo1RDY2MzFCMCIsInRpbWVzdGFtcCI6MTU2Njk3ODQ4MCwiaG9zdCI6ImdpdGh1Yi5jb20ifQ==">

    <meta name="enabled-features" content="ACTIONS_V2_ON_MARKETPLACE,MARKETPLACE_FEATURED_BLOG_POSTS,MARKETPLACE_INVOICED_BILLING,MARKETPLACE_SOCIAL_PROOF_CUSTOMERS,MARKETPLACE_TRENDING_SOCIAL_PROOF,MARKETPLACE_RECOMMENDATIONS,MARKETPLACE_PENDING_INSTALLATIONS">

  <meta name="html-safe-nonce" content="b7b6d8705c7c8087527895f622243670702ed7eb">

  <meta http-equiv="x-pjax-version" content="d2d26cca200c67d0513c4358ceeb44aa">
  

      <link href="https://github.com/a8m/golang-cheat-sheet/commits/master.atom" rel="alternate" title="Recent Commits to golang-cheat-sheet:master" type="application/atom+xml">

  <meta name="go-import" content="github.com/a8m/golang-cheat-sheet git https://github.com/a8m/golang-cheat-sheet.git">

  <meta name="octolytics-dimension-user_id" content="7413593" /><meta name="octolytics-dimension-user_login" content="a8m" /><meta name="octolytics-dimension-repository_id" content="16800723" /><meta name="octolytics-dimension-repository_nwo" content="a8m/golang-cheat-sheet" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="16800723" /><meta name="octolytics-dimension-repository_network_root_nwo" content="a8m/golang-cheat-sheet" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="false" />


    <link rel="canonical" href="https://github.com/a8m/golang-cheat-sheet/blob/master/README.md" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://github.githubassets.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" class="js-site-favicon" href="https://github.githubassets.com/favicon.ico">

<meta name="theme-color" content="#1e2327">





  <link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-out env-production page-responsive page-blob">
    

  <div class="position-relative js-header-wrapper ">
    <a href="#start-of-content" tabindex="1" class="px-2 py-4 bg-blue text-white show-on-focus js-skip-to-content">Skip to content</a>
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>

    
    
    


        <header class="Header-old header-logged-out js-details-container Details position-relative f4 py-2" role="banner">
  <div class="container-lg d-lg-flex flex-items-center p-responsive">
    <div class="d-flex flex-justify-between flex-items-center">
        <a class="mr-4" href="https://github.com/" aria-label="Homepage" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
          <svg height="32" class="octicon octicon-mark-github text-white" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
        </a>

          <div class="d-lg-none css-truncate css-truncate-target width-fit p-2">
            
              <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
    <a class="Header-link" href="/a8m">a8m</a>
    /
    <a class="Header-link" href="/a8m/golang-cheat-sheet">golang-cheat-sheet</a>


          </div>

        <div class="d-flex flex-items-center">
            <a href="/join?source=header-repo"
              class="d-inline-block d-lg-none f5 text-white no-underline border border-gray-dark rounded-2 px-2 py-1 mr-3 mr-sm-5"
              data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;site header&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="ba25fbd04ea7a5683d300a3c0227dda414cb878611801754510471d8a9dab45f"
              data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">
              Sign&nbsp;up
            </a>

          <button class="btn-link d-lg-none mt-1 js-details-target" type="button" aria-label="Toggle navigation" aria-expanded="false">
            <svg height="24" class="octicon octicon-three-bars text-white" viewBox="0 0 12 16" version="1.1" width="18" aria-hidden="true"><path fill-rule="evenodd" d="M11.41 9H.59C0 9 0 8.59 0 8c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zm0-4H.59C0 5 0 4.59 0 4c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zM.59 11H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1H.59C0 13 0 12.59 0 12c0-.59 0-1 .59-1z"/></svg>
          </button>
        </div>
    </div>

    <div class="HeaderMenu HeaderMenu--logged-out position-fixed top-0 right-0 bottom-0 height-fit position-lg-relative d-lg-flex flex-justify-between flex-items-center flex-auto">
      <div class="d-flex d-lg-none flex-justify-end border-bottom bg-gray-light p-3">
        <button class="btn-link js-details-target" type="button" aria-label="Toggle navigation" aria-expanded="false">
          <svg height="24" class="octicon octicon-x text-gray" viewBox="0 0 12 16" version="1.1" width="18" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
        </button>
      </div>

        <nav class="mt-0 px-3 px-lg-0 mb-5 mb-lg-0" aria-label="Global">
          <ul class="d-lg-flex list-style-none">
              <li class="d-block d-lg-flex flex-lg-nowrap flex-lg-items-center border-bottom border-lg-bottom-0 mr-0 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap d-block d-lg-inline-block">
                    Why GitHub?
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-absolute position-lg-relative">
                      <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>
                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 mt-0 pb-4 p-lg-4 position-relative position-lg-absolute left-0 left-lg-n4">
                    <a href="/features" class="py-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Features">Features <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a>
                    <ul class="list-style-none f5 pb-3">
                      <li class="edge-item-fix"><a href="/features/code-review/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Code review">Code review</a></li>
                      <li class="edge-item-fix"><a href="/features/project-management/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Project management">Project management</a></li>
                      <li class="edge-item-fix"><a href="/features/integrations" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Integrations">Integrations</a></li>
                      <li class="edge-item-fix"><a href="/features/actions" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Actions">Actions</a>
                          <li class="edge-item-fix"><a href="/features/package-registry" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Package Registry">Package registry</a>
                      <li class="edge-item-fix"><a href="/features#team-management" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Team management">Team management</a></li>
                      <li class="edge-item-fix"><a href="/features#social-coding" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Social coding">Social coding</a></li>
                      <li class="edge-item-fix"><a href="/features#documentation" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Documentation">Documentation</a></li>
                      <li class="edge-item-fix"><a href="/features#code-hosting" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Code hosting">Code hosting</a></li>
                    </ul>

                    <ul class="list-style-none mb-0 border-lg-top pt-lg-3">
                      <li class="edge-item-fix"><a href="/customer-stories" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Customer stories">Customer stories <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                      <li class="edge-item-fix"><a href="/security" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Security">Security <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>
                  </div>
                </details>
              </li>
              <li class="border-bottom border-lg-bottom-0 mr-0 mr-lg-3">
                <a href="/enterprise" class="HeaderMenu-link no-underline py-3 d-block d-lg-inline-block" data-ga-click="(Logged out) Header, go to Enterprise">Enterprise</a>
              </li>

              <li class="d-block d-lg-flex flex-lg-nowrap flex-lg-items-center border-bottom border-lg-bottom-0 mr-0 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap d-block d-lg-inline-block">
                    Explore
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-absolute position-lg-relative">
                      <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>

                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 pt-2 pb-0 mt-0 pb-4 p-lg-4 position-relative position-lg-absolute left-0 left-lg-n4">
                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/explore" class="py-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Explore">Explore GitHub <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>

                    <h4 class="text-gray-light text-normal text-mono f5 mb-2 border-lg-top pt-lg-3">Learn &amp; contribute</h4>
                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/topics" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Topics">Topics</a></li>
                        <li class="edge-item-fix"><a href="/collections" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Collections">Collections</a></li>
                      <li class="edge-item-fix"><a href="/trending" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Trending">Trending</a></li>
                      <li class="edge-item-fix"><a href="https://lab.github.com/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Learning lab">Learning Lab</a></li>
                      <li class="edge-item-fix"><a href="https://opensource.guide" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Open source guides">Open source guides</a></li>
                    </ul>

                    <h4 class="text-gray-light text-normal text-mono f5 mb-2 border-lg-top pt-lg-3">Connect with others</h4>
                    <ul class="list-style-none mb-0">
                      <li class="edge-item-fix"><a href="https://github.com/events" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Events">Events</a></li>
                      <li class="edge-item-fix"><a href="https://github.community" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Community forum">Community forum</a></li>
                      <li class="edge-item-fix"><a href="https://education.github.com" class="py-2 pb-0 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to GitHub Education">GitHub Education</a></li>
                    </ul>
                  </div>
                </details>
              </li>

              <li class="border-bottom border-lg-bottom-0 mr-0 mr-lg-3">
                <a href="/marketplace" class="HeaderMenu-link no-underline py-3 d-block d-lg-inline-block" data-ga-click="(Logged out) Header, go to Marketplace">Marketplace</a>
              </li>

              <li class="d-block d-lg-flex flex-lg-nowrap flex-lg-items-center border-bottom border-lg-bottom-0 mr-0 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap d-block d-lg-inline-block">
                    Pricing
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-absolute position-lg-relative">
                       <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>

                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 pt-2 pb-4 mt-0 p-lg-4 position-relative position-lg-absolute left-0 left-lg-n4">
                    <a href="/pricing" class="pb-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Pricing">Plans <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a>

                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/pricing#feature-comparison" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Compare plans">Compare plans</a></li>
                      <li class="edge-item-fix"><a href="https://enterprise.github.com/contact" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Contact Sales">Contact Sales</a></li>
                    </ul>

                    <ul class="list-style-none mb-0 border-lg-top pt-lg-3">
                      <li class="edge-item-fix"><a href="/nonprofit" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Nonprofits">Nonprofit <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                      <li class="edge-item-fix"><a href="https://education.github.com" class="py-2 pb-0 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover"  data-ga-click="(Logged out) Header, go to Education">Education <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>
                  </div>
                </details>
              </li>
          </ul>
        </nav>

      <div class="d-lg-flex flex-items-center px-3 px-lg-0 text-center text-lg-left">
          <div class="d-lg-flex mb-3 mb-lg-0">
            <div class="header-search flex-self-stretch flex-lg-self-auto mr-0 mr-lg-3 mb-3 mb-lg-0 scoped-search site-scoped-search js-site-search position-relative js-jump-to"
  role="combobox"
  aria-owns="jump-to-results"
  aria-label="Search or jump to"
  aria-haspopup="listbox"
  aria-expanded="false"
>
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" role="search" aria-label="Site" data-scope-type="Repository" data-scope-id="16800723" data-scoped-search-url="/a8m/golang-cheat-sheet/search" data-unscoped-search-url="/search" action="/a8m/golang-cheat-sheet/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
      <label class="form-control input-sm header-search-wrapper p-0 header-search-wrapper-jump-to position-relative d-flex flex-justify-between flex-items-center js-chromeless-input-container">
        <input type="text"
          class="form-control input-sm header-search-input jump-to-field js-jump-to-field js-site-search-focus js-site-search-field is-clearable"
          data-hotkey="s,/"
          name="q"
          value=""
          placeholder="Search"
          data-unscoped-placeholder="Search GitHub"
          data-scoped-placeholder="Search"
          autocapitalize="off"
          aria-autocomplete="list"
          aria-controls="jump-to-results"
          aria-label="Search"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations#csrf-token=NG9HPiNAcwwyZnw4XGBS6zwBmApEJAGU3FrDiYNNnY8D1gdW/qu8QqL4F+iEoyyoHEDy7+YuEPq5s0qPXqwIxg=="
          spellcheck="false"
          autocomplete="off"
          >
          <input type="hidden" class="js-site-search-type-field" name="type" >
            <img src="https://github.githubassets.com/images/search-key-slash.svg" alt="" class="mr-2 header-search-key-slash">

            <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
              
<ul class="d-none js-jump-to-suggestions-template-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-suggestion" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

</ul>

<ul class="d-none js-jump-to-no-results-template-container">
  <li class="d-flex flex-justify-center flex-items-center f5 d-none js-jump-to-suggestion p-2">
    <span class="text-gray">No suggested jump to results</span>
  </li>
</ul>

<ul id="jump-to-results" role="listbox" class="p-0 m-0 js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-scoped-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-global-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>


</ul>

            </div>
      </label>
</form>  </div>
</div>

          </div>

        <a href="/login?return_to=%2Fa8m%2Fgolang-cheat-sheet%2Fblob%2Fmaster%2FREADME.md"
          class="HeaderMenu-link no-underline mr-3"
          data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;site header menu&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="380f676697d5cd58f875214d26f455bf879425468d333e64016b0c30bc13d9ac"
          data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">
          Sign&nbsp;in
        </a>
          <a href="/join?source=header-repo"
            class="HeaderMenu-link d-inline-block no-underline border border-gray-dark rounded-1 px-2 py-1"
            data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;site header menu&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="380f676697d5cd58f875214d26f455bf879425468d333e64016b0c30bc13d9ac"
            data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">
            Sign&nbsp;up
          </a>
      </div>
    </div>
  </div>
</header>

  </div>

  <div id="start-of-content" class="show-on-focus"></div>


    <div id="js-flash-container">

</div>



  <div class="application-main " data-commit-hovercards-enabled>
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <main  >
      


  










  <div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav pt-0 pt-lg-4 ">
    <div class="repohead-details-container clearfix container-lg p-responsive d-none d-lg-block">

      <ul class="pagehead-actions">




  <li>
    
  <a class="tooltipped tooltipped-s btn btn-sm btn-with-count" aria-label="You must be signed in to watch a repository" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;notification subscription menu watch&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;LOG_IN&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="8ce59b84527dc2f980e8f873cba91de909296e14f74bd18578a3a4f1f2a8aa45" href="/login?return_to=%2Fa8m%2Fgolang-cheat-sheet">
    <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
    Watch
</a>    <a class="social-count" href="/a8m/golang-cheat-sheet/watchers"
       aria-label="163 users are watching this repository">
      163
    </a>

  </li>

  <li>
        <a class="btn btn-sm btn-with-count tooltipped tooltipped-s" aria-label="You must be signed in to star a repository" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;star button&quot;,&quot;repository_id&quot;:16800723,&quot;auth_type&quot;:&quot;LOG_IN&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="bb4505c096e596728a78b08d8bdf6464d78d84dae6812afa252865d7de087e41" href="/login?return_to=%2Fa8m%2Fgolang-cheat-sheet">
      <svg class="octicon octicon-star v-align-text-bottom" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
      Star
</a>
    <a class="social-count js-social-count" href="/a8m/golang-cheat-sheet/stargazers"
      aria-label="4073 users starred this repository">
      4,073
    </a>

  </li>

  <li>
      <a class="btn btn-sm btn-with-count tooltipped tooltipped-s" aria-label="You must be signed in to fork a repository" rel="nofollow" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;repo details fork button&quot;,&quot;repository_id&quot;:16800723,&quot;auth_type&quot;:&quot;LOG_IN&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="58399321cdc6745694018e95b1b7234989df945d70a33d92ad5459ee08263e00" href="/login?return_to=%2Fa8m%2Fgolang-cheat-sheet">
        <svg class="octicon octicon-repo-forked v-align-text-bottom" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
        Fork
</a>
    <a href="/a8m/golang-cheat-sheet/network/members" class="social-count"
       aria-label="543 users forked this repository">
      543
    </a>
  </li>
</ul>

      <h1 class="public ">
    <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a class="url fn" rel="author" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=7413593" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m">a8m</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a data-pjax="#js-repo-pjax-container" href="/a8m/golang-cheat-sheet">golang-cheat-sheet</a></strong>
  

</h1>

    </div>
    
<nav class="hx_reponav reponav js-repo-nav js-sidenav-container-pjax container-lg p-responsive d-none d-lg-block"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
    aria-label="Repository"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a class="js-selected-navigation-item selected reponav-item" itemprop="url" data-hotkey="g c" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /a8m/golang-cheat-sheet" href="/a8m/golang-cheat-sheet">
      <svg class="octicon octicon-code" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" data-hotkey="g i" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /a8m/golang-cheat-sheet/issues" href="/a8m/golang-cheat-sheet/issues">
        <svg class="octicon octicon-issue-opened" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="Counter">10</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a data-hotkey="g p" itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /a8m/golang-cheat-sheet/pulls" href="/a8m/golang-cheat-sheet/pulls">
      <svg class="octicon octicon-git-pull-request" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">1</span>
      <meta itemprop="position" content="3">
</a>  </span>


    <a data-hotkey="g b" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /a8m/golang-cheat-sheet/projects" href="/a8m/golang-cheat-sheet/projects">
      <svg class="octicon octicon-project" viewBox="0 0 15 16" version="1.1" width="15" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      Projects
      <span class="Counter" >0</span>
</a>


    <a data-skip-pjax="true" class="js-selected-navigation-item reponav-item" data-selected-links="security alerts policy /a8m/golang-cheat-sheet/security/advisories" href="/a8m/golang-cheat-sheet/security/advisories">
      <svg class="octicon octicon-shield" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 2l7-2 7 2v6.02C14 12.69 8.69 16 7 16c-1.69 0-7-3.31-7-7.98V2zm1 .75L7 1l6 1.75v5.268C13 12.104 8.449 15 7 15c-1.449 0-6-2.896-6-6.982V2.75zm1 .75L7 2v12c-1.207 0-5-2.482-5-5.985V3.5z"/></svg>
      Security
</a>
    <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors dependency_graph pulse people /a8m/golang-cheat-sheet/pulse" href="/a8m/golang-cheat-sheet/pulse">
      <svg class="octicon octicon-graph" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
      Insights
</a>

</nav>

  <div class="reponav-wrapper reponav-small d-lg-none">
  <nav class="reponav js-reponav text-center no-wrap"
       itemscope
       itemtype="http://schema.org/BreadcrumbList">

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a class="js-selected-navigation-item selected reponav-item" itemprop="url" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /a8m/golang-cheat-sheet" href="/a8m/golang-cheat-sheet">
        <span itemprop="name">Code</span>
        <meta itemprop="position" content="1">
</a>    </span>

      <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
        <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /a8m/golang-cheat-sheet/issues" href="/a8m/golang-cheat-sheet/issues">
          <span itemprop="name">Issues</span>
          <span class="Counter">10</span>
          <meta itemprop="position" content="2">
</a>      </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /a8m/golang-cheat-sheet/pulls" href="/a8m/golang-cheat-sheet/pulls">
        <span itemprop="name">Pull requests</span>
        <span class="Counter">1</span>
        <meta itemprop="position" content="3">
</a>    </span>

      <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
        <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /a8m/golang-cheat-sheet/projects" href="/a8m/golang-cheat-sheet/projects">
          <span itemprop="name">Projects</span>
          <span class="Counter">0</span>
          <meta itemprop="position" content="4">
</a>      </span>


      <a itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="security alerts policy /a8m/golang-cheat-sheet/security/advisories" href="/a8m/golang-cheat-sheet/security/advisories">
        <span itemprop="name">Security</span>
        <meta itemprop="position" content="6">
</a>
      <a class="js-selected-navigation-item reponav-item" data-selected-links="pulse /a8m/golang-cheat-sheet/pulse" href="/a8m/golang-cheat-sheet/pulse">
        Pulse
</a>

  </nav>
</div>


  </div>
<div class="container-lg clearfix new-discussion-timeline experiment-repo-nav  p-responsive">
  <div class="repository-content ">

    
    


  


    <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/a8m/golang-cheat-sheet/blob/281456992efcb99d0423e6fc6c6ed297252a78e1/README.md">Permalink</a>

    <!-- blob contrib key: blob_contributors:v21:93ebd0da45dc28259bbf4f3cccdf3d39 -->
          <div class="signup-prompt-bg rounded-1">
      <div class="signup-prompt p-4 text-center mb-4 rounded-1">
        <div class="position-relative">
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form action="/prompt_dismissals/signup" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="_method" value="put" /><input type="hidden" name="authenticity_token" value="+j3m/jqBTtLs500UCsQuD6Uj9eR54UmgKaWRKa5lxtIxfN6obPcnuRWx4N9LAK6o24fcjtFxfnE9vVU7/TbRaw==" />
            <button type="submit" class="position-absolute top-0 right-0 btn-link link-gray" data-ga-click="(Logged out) Sign up prompt, clicked Dismiss, text:dismiss">
              Dismiss
            </button>
</form>          <h3 class="pt-2">Join GitHub today</h3>
          <p class="col-6 mx-auto">GitHub is home to over 40 million developers working together to host and review code, manage projects, and build software together.</p>
          <a class="btn btn-primary" data-hydro-click="{&quot;event_type&quot;:&quot;authentication.click&quot;,&quot;payload&quot;:{&quot;location_in_page&quot;:&quot;files signup prompt&quot;,&quot;repository_id&quot;:null,&quot;auth_type&quot;:&quot;SIGN_UP&quot;,&quot;client_id&quot;:null,&quot;originating_request_id&quot;:&quot;A8AA:0B56:311D8D:450C23:5D6631B0&quot;,&quot;originating_url&quot;:&quot;https://github.com/a8m/golang-cheat-sheet/blob/master/README.md&quot;,&quot;referrer&quot;:null,&quot;user_id&quot;:null}}" data-hydro-click-hmac="869c4cfade0b0a851db8f6cb36a5e5b824f7c030aff051a394af2037b6658671" data-ga-click="(Logged out) Sign up prompt, clicked Sign up, text:sign-up" href="/join?source=prompt-blob-show">Sign up</a>
        </div>
      </div>
    </div>


    <div class="d-flex flex-items-start flex-shrink-0 pb-3 flex-column flex-md-row">
      <span class="d-flex flex-justify-between width-full width-md-auto">
        
<details class="details-reset details-overlay select-menu branch-select-menu  hx_rsm" id="branch-select-menu">
  <summary class="btn btn-sm select-menu-button css-truncate"
           data-hotkey="w"
           title="Switch branches or tags">
    <i>Branch:</i>
    <span class="css-truncate-target" data-menu-button>master</span>
  </summary>

  <details-menu class="select-menu-modal hx_rsm-modal position-absolute" style="z-index: 99;" src="/a8m/golang-cheat-sheet/ref-list/master/README.md?source_action=show&amp;source_controller=blob" preload>
    <include-fragment class="select-menu-loading-overlay anim-pulse">
      <svg height="32" class="octicon octicon-octoface" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M14.7 5.34c.13-.32.55-1.59-.13-3.31 0 0-1.05-.33-3.44 1.3-1-.28-2.07-.32-3.13-.32s-2.13.04-3.13.32c-2.39-1.64-3.44-1.3-3.44-1.3-.68 1.72-.26 2.99-.13 3.31C.49 6.21 0 7.33 0 8.69 0 13.84 3.33 15 7.98 15S16 13.84 16 8.69c0-1.36-.49-2.48-1.3-3.35zM8 14.02c-3.3 0-5.98-.15-5.98-3.35 0-.76.38-1.48 1.02-2.07 1.07-.98 2.9-.46 4.96-.46 2.07 0 3.88-.52 4.96.46.65.59 1.02 1.3 1.02 2.07 0 3.19-2.68 3.35-5.98 3.35zM5.49 9.01c-.66 0-1.2.8-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.54-1.78-1.2-1.78zm5.02 0c-.66 0-1.2.79-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.53-1.78-1.2-1.78z"/></svg>
    </include-fragment>
  </details-menu>
</details>

        <div class="BtnGroup flex-shrink-0 d-md-none">
          <a href="/a8m/golang-cheat-sheet/find/master"
                class="js-pjax-capture-input btn btn-sm BtnGroup-item"
                data-pjax
                data-hotkey="t">
            Find file
          </a>
          <clipboard-copy value="README.md" class="btn btn-sm BtnGroup-item">
            Copy path
          </clipboard-copy>
        </div>
      </span>
      <h2 id="blob-path" class="breadcrumb flex-auto min-width-0 text-normal flex-md-self-center ml-md-2 mr-md-3 my-2 my-md-0">
        <span class="js-repo-root text-bold"><span class="js-path-segment"><a data-pjax="true" href="/a8m/golang-cheat-sheet"><span>golang-cheat-sheet</span></a></span></span><span class="separator">/</span><strong class="final-path">README.md</strong>
      </h2>

      <div class="BtnGroup flex-shrink-0 d-none d-md-inline-block">
        <a href="/a8m/golang-cheat-sheet/find/master"
              class="js-pjax-capture-input btn btn-sm BtnGroup-item"
              data-pjax
              data-hotkey="t">
          Find file
        </a>
        <clipboard-copy value="README.md" class="btn btn-sm BtnGroup-item">
          Copy path
        </clipboard-copy>
      </div>
    </div>



    
  <div class="Box Box--condensed d-flex flex-column flex-shrink-0">
      <div class="Box-body d-flex flex-justify-between bg-blue-light flex-column flex-md-row flex-items-start flex-md-items-center">
        <span class="pr-md-4 f6">
          <a rel="contributor" data-skip-pjax="true" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=8470763" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/codingsince1985"><img class="avatar" src="https://avatars3.githubusercontent.com/u/8470763?s=40&amp;v=4" width="20" height="20" alt="@codingsince1985" /></a>
          <a class="text-bold link-gray-dark lh-default v-align-middle" rel="contributor" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=8470763" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/codingsince1985">codingsince1985</a>
            <span class="lh-default v-align-middle">
              <a data-pjax="true" title="example of iota

#57" class="link-gray" href="/a8m/golang-cheat-sheet/commit/a82a7d81393c29e1556aeda4031f8360ae45d10b">example of iota</a>
            </span>
        </span>
        <span class="d-inline-block flex-shrink-0 v-align-bottom f6 mt-2 mt-md-0">
          <a class="pr-2 text-mono link-gray" href="/a8m/golang-cheat-sheet/commit/a82a7d81393c29e1556aeda4031f8360ae45d10b" data-pjax>a82a7d8</a>
          <relative-time datetime="2019-02-18T02:56:35Z">Feb 18, 2019</relative-time>
        </span>
      </div>

    <div class="Box-body d-flex flex-items-center flex-auto f6 border-bottom-0 flex-wrap" >
      <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark float-left mr-2" id="blob_contributors_box">
        <summary class="btn-link">
          <span><strong>19</strong> contributors</span>
        </summary>
        <details-dialog
          class="Box Box--overlay d-flex flex-column anim-fade-in fast"
          aria-label="Users who have contributed to this file"
          src="/a8m/golang-cheat-sheet/contributors/master/README.md/list" preload>
          <div class="Box-header">
            <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
              <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
            </button>
            <h3 class="Box-title">
              Users who have contributed to this file
            </h3>
          </div>
          <include-fragment class="octocat-spinner my-3" aria-label="Loading..."></include-fragment>
        </details-dialog>
      </details>
        <span class="">
    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=896858" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=donbright">
      <img class="avatar mr-1" src="https://avatars1.githubusercontent.com/u/896858?s=40&amp;v=4" width="20" height="20" alt="@donbright" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=7413593" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=a8m">
      <img class="avatar mr-1" src="https://avatars0.githubusercontent.com/u/7413593?s=40&amp;v=4" width="20" height="20" alt="@a8m" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=8470763" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=codingsince1985">
      <img class="avatar mr-1" src="https://avatars3.githubusercontent.com/u/8470763?s=40&amp;v=4" width="20" height="20" alt="@codingsince1985" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=169160" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=zipizap">
      <img class="avatar mr-1" src="https://avatars1.githubusercontent.com/u/169160?s=40&amp;v=4" width="20" height="20" alt="@zipizap" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=3818079" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=StevenMaude">
      <img class="avatar mr-1" src="https://avatars3.githubusercontent.com/u/3818079?s=40&amp;v=4" width="20" height="20" alt="@StevenMaude" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=536947" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=johnlunney">
      <img class="avatar mr-1" src="https://avatars0.githubusercontent.com/u/536947?s=40&amp;v=4" width="20" height="20" alt="@johnlunney" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=39798426" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=imbubble">
      <img class="avatar mr-1" src="https://avatars1.githubusercontent.com/u/39798426?s=40&amp;v=4" width="20" height="20" alt="@imbubble" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=435857" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=edigu">
      <img class="avatar mr-1" src="https://avatars1.githubusercontent.com/u/435857?s=40&amp;v=4" width="20" height="20" alt="@edigu" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=1559756" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=xiaocong">
      <img class="avatar mr-1" src="https://avatars1.githubusercontent.com/u/1559756?s=40&amp;v=4" width="20" height="20" alt="@xiaocong" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=252023" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=vassilevsky">
      <img class="avatar mr-1" src="https://avatars2.githubusercontent.com/u/252023?s=40&amp;v=4" width="20" height="20" alt="@vassilevsky" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=608906" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=sourcesoft">
      <img class="avatar mr-1" src="https://avatars2.githubusercontent.com/u/608906?s=40&amp;v=4" width="20" height="20" alt="@sourcesoft" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=6213311" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=MarounMaroun">
      <img class="avatar mr-1" src="https://avatars3.githubusercontent.com/u/6213311?s=40&amp;v=4" width="20" height="20" alt="@MarounMaroun" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=168393" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=LordLandon">
      <img class="avatar mr-1" src="https://avatars2.githubusercontent.com/u/168393?s=40&amp;v=4" width="20" height="20" alt="@LordLandon" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=5501657" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=iamolegga">
      <img class="avatar mr-1" src="https://avatars3.githubusercontent.com/u/5501657?s=40&amp;v=4" width="20" height="20" alt="@iamolegga" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=14178318" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=lagebr">
      <img class="avatar mr-1" src="https://avatars0.githubusercontent.com/u/14178318?s=40&amp;v=4" width="20" height="20" alt="@lagebr" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=1892337" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=hylyh">
      <img class="avatar mr-1" src="https://avatars1.githubusercontent.com/u/1892337?s=40&amp;v=4" width="20" height="20" alt="@hylyh" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=32617" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=amiorin">
      <img class="avatar mr-1" src="https://avatars0.githubusercontent.com/u/32617?s=40&amp;v=4" width="20" height="20" alt="@amiorin" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=5057434" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=cemilcelik">
      <img class="avatar mr-1" src="https://avatars3.githubusercontent.com/u/5057434?s=40&amp;v=4" width="20" height="20" alt="@cemilcelik" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=6330344" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/a8m/golang-cheat-sheet/commits/master/README.md?author=amosipov">
      <img class="avatar mr-1" src="https://avatars2.githubusercontent.com/u/6330344?s=40&amp;v=4" width="20" height="20" alt="@amosipov" /> 
</a>
</span>

    </div>
  </div>





    <div class="Box mt-3 position-relative">
      
<div class="Box-header py-2 d-flex flex-column flex-shrink-0 flex-md-row flex-md-items-center">

  <div class="text-mono f6 flex-auto pr-3 flex-order-2 flex-md-order-1 mt-2 mt-md-0">
      751 lines (621 sloc)
      <span class="file-info-divider"></span>
    17.2 KB
  </div>

  <div class="d-flex py-1 py-md-0 flex-auto flex-order-1 flex-md-order-2 flex-sm-grow-0 flex-justify-between">

    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/a8m/golang-cheat-sheet/raw/master/README.md">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/a8m/golang-cheat-sheet/blame/master/README.md">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/a8m/golang-cheat-sheet/commits/master/README.md">History</a>
    </div>


    <div>

          <button type="button" class="btn-octicon disabled tooltipped tooltipped-nw"
            aria-label="You must be signed in to make or propose changes">
            <svg class="octicon octicon-pencil" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
          </button>
          <button type="button" class="btn-octicon btn-octicon-danger disabled tooltipped tooltipped-nw"
            aria-label="You must be signed in to make or propose changes">
            <svg class="octicon octicon-trashcan" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
          </button>
    </div>
  </div>
</div>




      
  <div id="readme" class="Box-body readme blob instapaper_body js-code-block-container">
    <article class="markdown-body entry-content p-3 p-md-6" itemprop="text"><h1><a id="user-content-go-cheat-sheet" class="anchor" aria-hidden="true" href="#go-cheat-sheet"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Go Cheat Sheet</h1>
<h1><a id="user-content-index" class="anchor" aria-hidden="true" href="#index"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Index</h1>
<ol>
<li><a href="#basic-syntax">Basic Syntax</a></li>
<li><a href="#operators">Operators</a>
<ul>
<li><a href="#arithmetic">Arithmetic</a></li>
<li><a href="#comparison">Comparison</a></li>
<li><a href="#logical">Logical</a></li>
<li><a href="#other">Other</a></li>
</ul>
</li>
<li><a href="#declarations">Declarations</a></li>
<li><a href="#functions">Functions</a>
<ul>
<li><a href="#functions-as-values-and-closures">Functions as values and closures</a></li>
<li><a href="#variadic-functions">Variadic Functions</a></li>
</ul>
</li>
<li><a href="#built-in-types">Built-in Types</a></li>
<li><a href="#type-conversions">Type Conversions</a></li>
<li><a href="#packages">Packages</a></li>
<li><a href="#control-structures">Control structures</a>
<ul>
<li><a href="#if">If</a></li>
<li><a href="#loops">Loops</a></li>
<li><a href="#switch">Switch</a></li>
</ul>
</li>
<li><a href="#arrays-slices-ranges">Arrays, Slices, Ranges</a>
<ul>
<li><a href="#arrays">Arrays</a></li>
<li><a href="#slices">Slices</a></li>
<li><a href="#operations-on-arrays-and-slices">Operations on Arrays and Slices</a></li>
</ul>
</li>
<li><a href="#maps">Maps</a></li>
<li><a href="#structs">Structs</a></li>
<li><a href="#pointers">Pointers</a></li>
<li><a href="#interfaces">Interfaces</a></li>
<li><a href="#embedding">Embedding</a></li>
<li><a href="#errors">Errors</a></li>
<li><a href="#concurrency">Concurrency</a>
<ul>
<li><a href="#goroutines">Goroutines</a></li>
<li><a href="#channels">Channels</a></li>
<li><a href="#channel-axioms">Channel Axioms</a></li>
</ul>
</li>
<li><a href="#printing">Printing</a></li>
<li><a href="#reflection">Reflection</a>
<ul>
<li><a href="#type-switch">Type Switch</a></li>
<li><a href="https://github.com/a8m/reflect-examples">Examples</a></li>
</ul>
</li>
<li><a href="#snippets">Snippets</a>
<ul>
<li><a href="#http-server">Http-Server</a></li>
</ul>
</li>
</ol>
<h2><a id="user-content-credits" class="anchor" aria-hidden="true" href="#credits"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Credits</h2>
<p>Most example code taken from <a href="http://tour.golang.org/" rel="nofollow">A Tour of Go</a>, which is an excellent introduction to Go.
If you're new to Go, do that tour. Seriously.</p>
<h2><a id="user-content-go-in-a-nutshell" class="anchor" aria-hidden="true" href="#go-in-a-nutshell"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Go in a Nutshell</h2>
<ul>
<li>Imperative language</li>
<li>Statically typed</li>
<li>Syntax tokens similar to C (but less parentheses and no semicolons) and the structure to Oberon-2</li>
<li>Compiles to native code (no JVM)</li>
<li>No classes, but structs with methods</li>
<li>Interfaces</li>
<li>No implementation inheritance. There's <a href="http://golang.org/doc/effective%5Fgo.html#embedding" rel="nofollow">type embedding</a>, though.</li>
<li>Functions are first class citizens</li>
<li>Functions can return multiple values</li>
<li>Has closures</li>
<li>Pointers, but not pointer arithmetic</li>
<li>Built-in concurrency primitives: Goroutines and Channels</li>
</ul>
<h1><a id="user-content-basic-syntax" class="anchor" aria-hidden="true" href="#basic-syntax"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Basic Syntax</h1>
<h2><a id="user-content-hello-world" class="anchor" aria-hidden="true" href="#hello-world"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Hello World</h2>
<p>File <code>hello.go</code>:</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">package</span> main

<span class="pl-k">import</span> <span class="pl-s"><span class="pl-pds">"</span>fmt<span class="pl-pds">"</span></span>

<span class="pl-k">func</span> <span class="pl-en">main</span>() {
    fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Hello Go<span class="pl-pds">"</span></span>)
}</pre></div>
<p><code>$ go run hello.go</code></p>
<h2><a id="user-content-operators" class="anchor" aria-hidden="true" href="#operators"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Operators</h2>
<h3><a id="user-content-arithmetic" class="anchor" aria-hidden="true" href="#arithmetic"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Arithmetic</h3>
<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>+</code></td>
<td>addition</td>
</tr>
<tr>
<td><code>-</code></td>
<td>subtraction</td>
</tr>
<tr>
<td><code>*</code></td>
<td>multiplication</td>
</tr>
<tr>
<td><code>/</code></td>
<td>quotient</td>
</tr>
<tr>
<td><code>%</code></td>
<td>remainder</td>
</tr>
<tr>
<td><code>&amp;</code></td>
<td>bitwise and</td>
</tr>
<tr>
<td><code>|</code></td>
<td>bitwise or</td>
</tr>
<tr>
<td><code>^</code></td>
<td>bitwise xor</td>
</tr>
<tr>
<td><code>&amp;^</code></td>
<td>bit clear (and not)</td>
</tr>
<tr>
<td><code>&lt;&lt;</code></td>
<td>left shift</td>
</tr>
<tr>
<td><code>&gt;&gt;</code></td>
<td>right shift</td>
</tr>
</tbody>
</table>
<h3><a id="user-content-comparison" class="anchor" aria-hidden="true" href="#comparison"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Comparison</h3>
<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>==</code></td>
<td>equal</td>
</tr>
<tr>
<td><code>!=</code></td>
<td>not equal</td>
</tr>
<tr>
<td><code>&lt;</code></td>
<td>less than</td>
</tr>
<tr>
<td><code>&lt;=</code></td>
<td>less than or equal</td>
</tr>
<tr>
<td><code>&gt;</code></td>
<td>greater than</td>
</tr>
<tr>
<td><code>&gt;=</code></td>
<td>greater than or equal</td>
</tr>
</tbody>
</table>
<h3><a id="user-content-logical" class="anchor" aria-hidden="true" href="#logical"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logical</h3>
<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>&amp;&amp;</code></td>
<td>logical and</td>
</tr>
<tr>
<td><code>||</code></td>
<td>logical or</td>
</tr>
<tr>
<td><code>!</code></td>
<td>logical not</td>
</tr>
</tbody>
</table>
<h3><a id="user-content-other" class="anchor" aria-hidden="true" href="#other"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Other</h3>
<table>
<thead>
<tr>
<th>Operator</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>&amp;</code></td>
<td>address of / create pointer</td>
</tr>
<tr>
<td><code>*</code></td>
<td>dereference pointer</td>
</tr>
<tr>
<td><code>&lt;-</code></td>
<td>send / receive operator (see 'Channels' below)</td>
</tr>
</tbody>
</table>
<h2><a id="user-content-declarations" class="anchor" aria-hidden="true" href="#declarations"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Declarations</h2>
<p>Type goes after identifier!</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">foo</span> <span class="pl-k">int</span> <span class="pl-c"><span class="pl-c">//</span> declaration without initialization</span>
<span class="pl-k">var</span> <span class="pl-smi">foo</span> <span class="pl-k">int</span> = <span class="pl-c1">42</span> <span class="pl-c"><span class="pl-c">//</span> declaration with initialization</span>
<span class="pl-k">var</span> <span class="pl-smi">foo</span>, <span class="pl-smi">bar</span> <span class="pl-k">int</span> = <span class="pl-c1">42</span>, <span class="pl-c1">1302</span> <span class="pl-c"><span class="pl-c">//</span> declare and init multiple vars at once</span>
<span class="pl-k">var</span> <span class="pl-smi">foo</span> = <span class="pl-c1">42</span> <span class="pl-c"><span class="pl-c">//</span> type omitted, will be inferred</span>
<span class="pl-smi">foo</span> <span class="pl-k">:=</span> <span class="pl-c1">42</span> <span class="pl-c"><span class="pl-c">//</span> shorthand, only in func bodies, omit var keyword, type is always implicit</span>
<span class="pl-k">const</span> constant = <span class="pl-s"><span class="pl-pds">"</span>This is a constant<span class="pl-pds">"</span></span>

<span class="pl-c"><span class="pl-c">//</span> iota can be used for incrementing numbers, starting from 0</span>
<span class="pl-k">const</span> (
    _ = <span class="pl-c1">iota</span>
    a
    b
    c = <span class="pl-c1">1</span> &lt;&lt; <span class="pl-c1">iota</span>
    d
)
    fmt.<span class="pl-c1">Println</span>(a, b) <span class="pl-c"><span class="pl-c">//</span> 1 2 (0 is skipped)</span>
    fmt.<span class="pl-c1">Println</span>(c, d) <span class="pl-c"><span class="pl-c">//</span> 8 16 (2^3, 2^4)</span></pre></div>
<h2><a id="user-content-functions" class="anchor" aria-hidden="true" href="#functions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Functions</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-c"><span class="pl-c">//</span> a simple function</span>
<span class="pl-k">func</span> <span class="pl-en">functionName</span>() {}

<span class="pl-c"><span class="pl-c">//</span> function with parameters (again, types go after identifiers)</span>
<span class="pl-k">func</span> <span class="pl-en">functionName</span>(<span class="pl-v">param1</span> <span class="pl-v">string</span>, <span class="pl-v">param2</span> <span class="pl-v">int</span>) {}

<span class="pl-c"><span class="pl-c">//</span> multiple parameters of the same type</span>
<span class="pl-k">func</span> <span class="pl-en">functionName</span>(<span class="pl-v">param1</span>, <span class="pl-v">param2</span> <span class="pl-v">int</span>) {}

<span class="pl-c"><span class="pl-c">//</span> return type declaration</span>
<span class="pl-k">func</span> <span class="pl-en">functionName</span>() <span class="pl-v">int</span> {
    <span class="pl-k">return</span> <span class="pl-c1">42</span>
}

<span class="pl-c"><span class="pl-c">//</span> Can return multiple values at once</span>
<span class="pl-k">func</span> <span class="pl-en">returnMulti</span>() (<span class="pl-v">int</span>, <span class="pl-v">string</span>) {
    <span class="pl-k">return</span> <span class="pl-c1">42</span>, <span class="pl-s"><span class="pl-pds">"</span>foobar<span class="pl-pds">"</span></span>
}
<span class="pl-k">var</span> <span class="pl-smi">x</span>, <span class="pl-smi">str</span> = <span class="pl-c1">returnMulti</span>()

<span class="pl-c"><span class="pl-c">//</span> Return multiple named results simply by return</span>
<span class="pl-k">func</span> <span class="pl-en">returnMulti2</span>() (<span class="pl-v">n</span> <span class="pl-v">int</span>, <span class="pl-v">s</span> <span class="pl-v">string</span>) {
    n = <span class="pl-c1">42</span>
    s = <span class="pl-s"><span class="pl-pds">"</span>foobar<span class="pl-pds">"</span></span>
    <span class="pl-c"><span class="pl-c">//</span> n and s will be returned</span>
    <span class="pl-k">return</span>
}
<span class="pl-k">var</span> <span class="pl-smi">x</span>, <span class="pl-smi">str</span> = <span class="pl-c1">returnMulti2</span>()
</pre></div>
<h3><a id="user-content-functions-as-values-and-closures" class="anchor" aria-hidden="true" href="#functions-as-values-and-closures"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Functions As Values And Closures</h3>
<div class="highlight highlight-source-go"><pre><span class="pl-k">func</span> <span class="pl-en">main</span>() {
    <span class="pl-c"><span class="pl-c">//</span> assign a function to a name</span>
    <span class="pl-smi">add</span> <span class="pl-k">:=</span> <span class="pl-c1">func</span>(a, b <span class="pl-k">int</span>) <span class="pl-k">int</span> {
        <span class="pl-k">return</span> a + b
    }
    <span class="pl-c"><span class="pl-c">//</span> use the name to call the function</span>
    fmt.<span class="pl-c1">Println</span>(<span class="pl-c1">add</span>(<span class="pl-c1">3</span>, <span class="pl-c1">4</span>))
}

<span class="pl-c"><span class="pl-c">//</span> Closures, lexically scoped: Functions can access values that were</span>
<span class="pl-c"><span class="pl-c">//</span> in scope when defining the function</span>
<span class="pl-k">func</span> <span class="pl-en">scope</span>() <span class="pl-v">func</span>() int{
    <span class="pl-smi">outer_var</span> <span class="pl-k">:=</span> <span class="pl-c1">2</span>
    <span class="pl-smi">foo</span> <span class="pl-k">:=</span> <span class="pl-c1">func</span>() <span class="pl-k">int</span> { <span class="pl-k">return</span> outer_var}
    <span class="pl-k">return</span> foo
}

<span class="pl-k">func</span> <span class="pl-en">another_scope</span>() <span class="pl-v">func</span>() int{
    <span class="pl-c"><span class="pl-c">//</span> won't compile because outer_var and foo not defined in this scope</span>
    outer_var = <span class="pl-c1">444</span>
    <span class="pl-k">return</span> foo
}


<span class="pl-c"><span class="pl-c">//</span> Closures</span>
<span class="pl-k">func</span> <span class="pl-en">outer</span>() (<span class="pl-v">func</span>() int, int) {
    <span class="pl-smi">outer_var</span> <span class="pl-k">:=</span> <span class="pl-c1">2</span>
    <span class="pl-smi">inner</span> <span class="pl-k">:=</span> <span class="pl-c1">func</span>() <span class="pl-k">int</span> {
        outer_var += <span class="pl-c1">99</span> <span class="pl-c"><span class="pl-c">//</span> outer_var from outer scope is mutated.</span>
        <span class="pl-k">return</span> outer_var
    }
    <span class="pl-c1">inner</span>()
    <span class="pl-k">return</span> inner, outer_var <span class="pl-c"><span class="pl-c">//</span> return inner func and mutated outer_var 101</span>
}</pre></div>
<h3><a id="user-content-variadic-functions" class="anchor" aria-hidden="true" href="#variadic-functions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Variadic Functions</h3>
<div class="highlight highlight-source-go"><pre><span class="pl-k">func</span> <span class="pl-en">main</span>() {
	fmt.<span class="pl-c1">Println</span>(<span class="pl-c1">adder</span>(<span class="pl-c1">1</span>, <span class="pl-c1">2</span>, <span class="pl-c1">3</span>)) 	<span class="pl-c"><span class="pl-c">//</span> 6</span>
	fmt.<span class="pl-c1">Println</span>(<span class="pl-c1">adder</span>(<span class="pl-c1">9</span>, <span class="pl-c1">9</span>))	<span class="pl-c"><span class="pl-c">//</span> 18</span>

	<span class="pl-smi">nums</span> <span class="pl-k">:=</span> []<span class="pl-k">int</span>{<span class="pl-c1">10</span>, <span class="pl-c1">20</span>, <span class="pl-c1">30</span>}
	fmt.<span class="pl-c1">Println</span>(<span class="pl-c1">adder</span>(nums...))	<span class="pl-c"><span class="pl-c">//</span> 60</span>
}

<span class="pl-c"><span class="pl-c">//</span> By using ... before the type name of the last parameter you can indicate that it takes zero or more of those parameters.</span>
<span class="pl-c"><span class="pl-c">//</span> The function is invoked like any other function except we can pass as many arguments as we want.</span>
<span class="pl-k">func</span> <span class="pl-en">adder</span>(<span class="pl-v">args</span> ...<span class="pl-v">int</span>) <span class="pl-v">int</span> {
	<span class="pl-smi">total</span> <span class="pl-k">:=</span> <span class="pl-c1">0</span>
	<span class="pl-k">for</span> <span class="pl-smi">_</span>, <span class="pl-smi">v</span> <span class="pl-k">:=</span> <span class="pl-k">range</span> args { <span class="pl-c"><span class="pl-c">//</span> Iterates over the arguments whatever the number.</span>
		total += v
	}
	<span class="pl-k">return</span> total
}</pre></div>
<h2><a id="user-content-built-in-types" class="anchor" aria-hidden="true" href="#built-in-types"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Built-in Types</h2>
<pre><code>bool

string

int  int8  int16  int32  int64
uint uint8 uint16 uint32 uint64 uintptr

byte // alias for uint8

rune // alias for int32 ~= a character (Unicode code point) - very Viking

float32 float64

complex64 complex128
</code></pre>
<h2><a id="user-content-type-conversions" class="anchor" aria-hidden="true" href="#type-conversions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Type Conversions</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">i</span> <span class="pl-k">int</span> = <span class="pl-c1">42</span>
<span class="pl-k">var</span> <span class="pl-smi">f</span> <span class="pl-k">float64</span> = <span class="pl-c1">float64</span>(i)
<span class="pl-k">var</span> <span class="pl-smi">u</span> <span class="pl-k">uint</span> = <span class="pl-c1">uint</span>(f)

<span class="pl-c"><span class="pl-c">//</span> alternative syntax</span>
<span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-c1">42</span>
<span class="pl-smi">f</span> <span class="pl-k">:=</span> <span class="pl-c1">float64</span>(i)
<span class="pl-smi">u</span> <span class="pl-k">:=</span> <span class="pl-c1">uint</span>(f)</pre></div>
<h2><a id="user-content-packages" class="anchor" aria-hidden="true" href="#packages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Packages</h2>
<ul>
<li>Package declaration at top of every source file</li>
<li>Executables are in package <code>main</code></li>
<li>Convention: package name == last name of import path (import path <code>math/rand</code> =&gt; package <code>rand</code>)</li>
<li>Upper case identifier: exported (visible from other packages)</li>
<li>Lower case identifier: private (not visible from other packages)</li>
</ul>
<h2><a id="user-content-control-structures" class="anchor" aria-hidden="true" href="#control-structures"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Control structures</h2>
<h3><a id="user-content-if" class="anchor" aria-hidden="true" href="#if"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>If</h3>
<div class="highlight highlight-source-go"><pre><span class="pl-k">func</span> <span class="pl-en">main</span>() {
	<span class="pl-c"><span class="pl-c">//</span> Basic one</span>
	<span class="pl-k">if</span> x &gt; <span class="pl-c1">10</span> {
		<span class="pl-k">return</span> x
	} <span class="pl-k">else</span> <span class="pl-k">if</span> x == <span class="pl-c1">10</span> {
		<span class="pl-k">return</span> <span class="pl-c1">10</span>
	} <span class="pl-k">else</span> {
		<span class="pl-k">return</span> -x
	}

	<span class="pl-c"><span class="pl-c">//</span> You can put one statement before the condition</span>
	<span class="pl-k">if</span> <span class="pl-smi">a</span> <span class="pl-k">:=</span> b + c; a &lt; <span class="pl-c1">42</span> {
		<span class="pl-k">return</span> a
	} <span class="pl-k">else</span> {
		<span class="pl-k">return</span> a - <span class="pl-c1">42</span>
	}

	<span class="pl-c"><span class="pl-c">//</span> Type assertion inside if</span>
	<span class="pl-k">var</span> <span class="pl-smi">val</span> <span class="pl-k">interface</span>{}
	val = <span class="pl-s"><span class="pl-pds">"</span>foo<span class="pl-pds">"</span></span>
	<span class="pl-k">if</span> <span class="pl-smi">str</span>, <span class="pl-smi">ok</span> <span class="pl-k">:=</span> val.(<span class="pl-k">string</span>); ok {
		fmt.<span class="pl-c1">Println</span>(str)
	}
}</pre></div>
<h3><a id="user-content-loops" class="anchor" aria-hidden="true" href="#loops"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Loops</h3>
<div class="highlight highlight-source-go"><pre>    <span class="pl-c"><span class="pl-c">//</span> There's only `for`, no `while`, no `until`</span>
    <span class="pl-k">for</span> <span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-c1">1</span>; i &lt; <span class="pl-c1">10</span>; i++ {
    }
    <span class="pl-k">for</span> ; i &lt; <span class="pl-c1">10</span>;  { <span class="pl-c"><span class="pl-c">//</span> while - loop</span>
    }
    <span class="pl-k">for</span> i &lt; <span class="pl-c1">10</span>  { <span class="pl-c"><span class="pl-c">//</span> you can omit semicolons if there is only a condition</span>
    }
    <span class="pl-k">for</span> { <span class="pl-c"><span class="pl-c">//</span> you can omit the condition ~ while (true)</span>
    }
    
    <span class="pl-c"><span class="pl-c">//</span> use break/continue on current loop</span>
    <span class="pl-c"><span class="pl-c">//</span> use break/continue with label on outer loop</span>
here:
    <span class="pl-k">for</span> <span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-c1">0</span>; i &lt; <span class="pl-c1">2</span>; i++ {
        <span class="pl-k">for</span> <span class="pl-smi">j</span> <span class="pl-k">:=</span> i + <span class="pl-c1">1</span>; j &lt; <span class="pl-c1">3</span>; j++ {
            <span class="pl-k">if</span> i == <span class="pl-c1">0</span> {
                <span class="pl-k">continue</span> here
            }
            fmt.<span class="pl-c1">Println</span>(j)
            <span class="pl-k">if</span> j == <span class="pl-c1">2</span> {
                <span class="pl-k">break</span>
            }
        }
    }

there:
    <span class="pl-k">for</span> <span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-c1">0</span>; i &lt; <span class="pl-c1">2</span>; i++ {
        <span class="pl-k">for</span> <span class="pl-smi">j</span> <span class="pl-k">:=</span> i + <span class="pl-c1">1</span>; j &lt; <span class="pl-c1">3</span>; j++ {
            <span class="pl-k">if</span> j == <span class="pl-c1">1</span> {
                <span class="pl-k">continue</span>
            }
            fmt.<span class="pl-c1">Println</span>(j)
            <span class="pl-k">if</span> j == <span class="pl-c1">2</span> {
                <span class="pl-k">break</span> there
            }
        }
    }</pre></div>
<h3><a id="user-content-switch" class="anchor" aria-hidden="true" href="#switch"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Switch</h3>
<div class="highlight highlight-source-go"><pre>    <span class="pl-c"><span class="pl-c">//</span> switch statement</span>
    <span class="pl-k">switch</span> operatingSystem {
    <span class="pl-k">case</span> <span class="pl-s"><span class="pl-pds">"</span>darwin<span class="pl-pds">"</span></span>:
        fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Mac OS Hipster<span class="pl-pds">"</span></span>)
        <span class="pl-c"><span class="pl-c">//</span> cases break automatically, no fallthrough by default</span>
    <span class="pl-k">case</span> <span class="pl-s"><span class="pl-pds">"</span>linux<span class="pl-pds">"</span></span>:
        fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Linux Geek<span class="pl-pds">"</span></span>)
    <span class="pl-k">default</span>:
        <span class="pl-c"><span class="pl-c">//</span> Windows, BSD, ...</span>
        fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Other<span class="pl-pds">"</span></span>)
    }

    <span class="pl-c"><span class="pl-c">//</span> as with for and if, you can have an assignment statement before the switch value</span>
    <span class="pl-k">switch</span> <span class="pl-smi">os</span> <span class="pl-k">:=</span> runtime.<span class="pl-smi">GOOS</span>; os {
    <span class="pl-k">case</span> <span class="pl-s"><span class="pl-pds">"</span>darwin<span class="pl-pds">"</span></span>: ...
    }

    <span class="pl-c"><span class="pl-c">//</span> you can also make comparisons in switch cases</span>
    <span class="pl-smi">number</span> <span class="pl-k">:=</span> <span class="pl-c1">42</span>
    <span class="pl-k">switch</span> {
        <span class="pl-k">case</span> number &lt; <span class="pl-c1">42</span>:
            fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Smaller<span class="pl-pds">"</span></span>)
        <span class="pl-k">case</span> number == <span class="pl-c1">42</span>:
            fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Equal<span class="pl-pds">"</span></span>)
        <span class="pl-k">case</span> number &gt; <span class="pl-c1">42</span>:
            fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Greater<span class="pl-pds">"</span></span>)
    }

    <span class="pl-c"><span class="pl-c">//</span> cases can be presented in comma-separated lists</span>
    <span class="pl-k">var</span> <span class="pl-smi">char</span> <span class="pl-k">byte</span> = <span class="pl-s"><span class="pl-pds">'</span>?<span class="pl-pds">'</span></span>
    <span class="pl-k">switch</span> char {
        <span class="pl-k">case</span> <span class="pl-s"><span class="pl-pds">'</span> <span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>?<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>&amp;<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>=<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>#<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>+<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>%<span class="pl-pds">'</span></span>:
            fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Should escape<span class="pl-pds">"</span></span>)
    }</pre></div>
<h2><a id="user-content-arrays-slices-ranges" class="anchor" aria-hidden="true" href="#arrays-slices-ranges"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Arrays, Slices, Ranges</h2>
<h3><a id="user-content-arrays" class="anchor" aria-hidden="true" href="#arrays"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Arrays</h3>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">a</span> [<span class="pl-c1">10</span>]<span class="pl-k">int</span> <span class="pl-c"><span class="pl-c">//</span> declare an int array with length 10. Array length is part of the type!</span>
a[<span class="pl-c1">3</span>] = <span class="pl-c1">42</span>     <span class="pl-c"><span class="pl-c">//</span> set elements</span>
<span class="pl-smi">i</span> <span class="pl-k">:=</span> a[<span class="pl-c1">3</span>]     <span class="pl-c"><span class="pl-c">//</span> read elements</span>

<span class="pl-c"><span class="pl-c">//</span> declare and initialize</span>
<span class="pl-k">var</span> <span class="pl-smi">a</span> = [<span class="pl-c1">2</span>]<span class="pl-k">int</span>{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>}
<span class="pl-smi">a</span> <span class="pl-k">:=</span> [<span class="pl-c1">2</span>]<span class="pl-k">int</span>{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>} <span class="pl-c"><span class="pl-c">//</span>shorthand</span>
<span class="pl-smi">a</span> <span class="pl-k">:=</span> [...]<span class="pl-k">int</span>{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>} <span class="pl-c"><span class="pl-c">//</span> elipsis -&gt; Compiler figures out array length</span></pre></div>
<h3><a id="user-content-slices" class="anchor" aria-hidden="true" href="#slices"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Slices</h3>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">a</span> []<span class="pl-k">int</span>                              <span class="pl-c"><span class="pl-c">//</span> declare a slice - similar to an array, but length is unspecified</span>
<span class="pl-k">var</span> <span class="pl-smi">a</span> = []<span class="pl-k">int</span> {<span class="pl-c1">1</span>, <span class="pl-c1">2</span>, <span class="pl-c1">3</span>, <span class="pl-c1">4</span>}               <span class="pl-c"><span class="pl-c">//</span> declare and initialize a slice (backed by the array given implicitly)</span>
<span class="pl-smi">a</span> <span class="pl-k">:=</span> []<span class="pl-k">int</span>{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>, <span class="pl-c1">3</span>, <span class="pl-c1">4</span>}                   <span class="pl-c"><span class="pl-c">//</span> shorthand</span>
<span class="pl-smi">chars</span> <span class="pl-k">:=</span> []<span class="pl-k">string</span>{<span class="pl-c1">0</span>:<span class="pl-s"><span class="pl-pds">"</span>a<span class="pl-pds">"</span></span>, <span class="pl-c1">2</span>:<span class="pl-s"><span class="pl-pds">"</span>c<span class="pl-pds">"</span></span>, <span class="pl-c1">1</span>: <span class="pl-s"><span class="pl-pds">"</span>b<span class="pl-pds">"</span></span>}  <span class="pl-c"><span class="pl-c">//</span> ["a", "b", "c"]</span>

<span class="pl-k">var</span> <span class="pl-smi">b</span> = a[lo:hi]	<span class="pl-c"><span class="pl-c">//</span> creates a slice (view of the array) from index lo to hi-1</span>
<span class="pl-k">var</span> <span class="pl-smi">b</span> = a[<span class="pl-c1">1</span>:<span class="pl-c1">4</span>]		<span class="pl-c"><span class="pl-c">//</span> slice from index 1 to 3</span>
<span class="pl-k">var</span> <span class="pl-smi">b</span> = a[:<span class="pl-c1">3</span>]		<span class="pl-c"><span class="pl-c">//</span> missing low index implies 0</span>
<span class="pl-k">var</span> <span class="pl-smi">b</span> = a[<span class="pl-c1">3</span>:]		<span class="pl-c"><span class="pl-c">//</span> missing high index implies len(a)</span>
a =  <span class="pl-c1">append</span>(a,<span class="pl-c1">17</span>,<span class="pl-c1">3</span>)	<span class="pl-c"><span class="pl-c">//</span> append items to slice a</span>
<span class="pl-smi">c</span> <span class="pl-k">:=</span> <span class="pl-c1">append</span>(a,b...)	<span class="pl-c"><span class="pl-c">//</span> concatenate slices a and b</span>

<span class="pl-c"><span class="pl-c">//</span> create a slice with make</span>
a = <span class="pl-c1">make</span>([]<span class="pl-k">byte</span>, <span class="pl-c1">5</span>, <span class="pl-c1">5</span>)	<span class="pl-c"><span class="pl-c">//</span> first arg length, second capacity</span>
a = <span class="pl-c1">make</span>([]<span class="pl-k">byte</span>, <span class="pl-c1">5</span>)	<span class="pl-c"><span class="pl-c">//</span> capacity is optional</span>

<span class="pl-c"><span class="pl-c">//</span> create a slice from an array</span>
<span class="pl-smi">x</span> <span class="pl-k">:=</span> [<span class="pl-c1">3</span>]<span class="pl-k">string</span>{<span class="pl-s"><span class="pl-pds">"</span>Лайка<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Белка<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Стрелка<span class="pl-pds">"</span></span>}
<span class="pl-smi">s</span> <span class="pl-k">:=</span> x[:] <span class="pl-c"><span class="pl-c">//</span> a slice referencing the storage of x</span></pre></div>
<h3><a id="user-content-operations-on-arrays-and-slices" class="anchor" aria-hidden="true" href="#operations-on-arrays-and-slices"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Operations on Arrays and Slices</h3>
<p><code>len(a)</code> gives you the length of an array/a slice. It's a built-in function, not a attribute/method on the array.</p>
<div class="highlight highlight-source-go"><pre><span class="pl-c"><span class="pl-c">//</span> loop over an array/a slice</span>
<span class="pl-k">for</span> <span class="pl-smi">i</span>, <span class="pl-smi">e</span> <span class="pl-k">:=</span> <span class="pl-k">range</span> a {
    <span class="pl-c"><span class="pl-c">//</span> i is the index, e the element</span>
}

<span class="pl-c"><span class="pl-c">//</span> if you only need e:</span>
<span class="pl-k">for</span> <span class="pl-smi">_</span>, <span class="pl-smi">e</span> <span class="pl-k">:=</span> <span class="pl-k">range</span> a {
    <span class="pl-c"><span class="pl-c">//</span> e is the element</span>
}

<span class="pl-c"><span class="pl-c">//</span> ...and if you only need the index</span>
<span class="pl-k">for</span> <span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-k">range</span> a {
}

<span class="pl-c"><span class="pl-c">//</span> In Go pre-1.4, you'll get a compiler error if you're not using i and e.</span>
<span class="pl-c"><span class="pl-c">//</span> Go 1.4 introduced a variable-free form, so that you can do this</span>
<span class="pl-k">for</span> <span class="pl-k">range</span> time.<span class="pl-c1">Tick</span>(time.<span class="pl-smi">Second</span>) {
    <span class="pl-c"><span class="pl-c">//</span> do it once a sec</span>
}
</pre></div>
<h2><a id="user-content-maps" class="anchor" aria-hidden="true" href="#maps"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Maps</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">m</span> <span class="pl-k">map</span>[<span class="pl-k">string</span>]<span class="pl-k">int</span>
m = <span class="pl-c1">make</span>(<span class="pl-k">map</span>[<span class="pl-k">string</span>]<span class="pl-k">int</span>)
m[<span class="pl-s"><span class="pl-pds">"</span>key<span class="pl-pds">"</span></span>] = <span class="pl-c1">42</span>
fmt.<span class="pl-c1">Println</span>(m[<span class="pl-s"><span class="pl-pds">"</span>key<span class="pl-pds">"</span></span>])

<span class="pl-c1">delete</span>(m, <span class="pl-s"><span class="pl-pds">"</span>key<span class="pl-pds">"</span></span>)

<span class="pl-smi">elem</span>, <span class="pl-smi">ok</span> <span class="pl-k">:=</span> m[<span class="pl-s"><span class="pl-pds">"</span>key<span class="pl-pds">"</span></span>] <span class="pl-c"><span class="pl-c">//</span> test if key "key" is present and retrieve it, if so</span>

<span class="pl-c"><span class="pl-c">//</span> map literal</span>
<span class="pl-k">var</span> <span class="pl-smi">m</span> = <span class="pl-k">map</span>[<span class="pl-k">string</span>]Vertex{
    <span class="pl-s"><span class="pl-pds">"</span>Bell Labs<span class="pl-pds">"</span></span>: {<span class="pl-c1">40.68433</span>, -<span class="pl-c1">74.39967</span>},
    <span class="pl-s"><span class="pl-pds">"</span>Google<span class="pl-pds">"</span></span>:    {<span class="pl-c1">37.42202</span>, -<span class="pl-c1">122.08408</span>},
}

<span class="pl-c"><span class="pl-c">//</span> iterate over map content</span>
<span class="pl-k">for</span> <span class="pl-smi">key</span>, <span class="pl-smi">value</span> <span class="pl-k">:=</span> <span class="pl-k">range</span> m {
}
</pre></div>
<h2><a id="user-content-structs" class="anchor" aria-hidden="true" href="#structs"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Structs</h2>
<p>There are no classes, only structs. Structs can have methods.</p>
<div class="highlight highlight-source-go"><pre><span class="pl-c"><span class="pl-c">//</span> A struct is a type. It's also a collection of fields</span>

<span class="pl-c"><span class="pl-c">//</span> Declaration</span>
<span class="pl-k">type</span> <span class="pl-v">Vertex</span> <span class="pl-k">struct</span> {
    <span class="pl-v">X</span>, <span class="pl-v">Y</span> <span class="pl-k">int</span>
}

<span class="pl-c"><span class="pl-c">//</span> Creating</span>
<span class="pl-k">var</span> <span class="pl-smi">v</span> = <span class="pl-v">Vertex</span>{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>}
<span class="pl-k">var</span> <span class="pl-smi">v</span> = <span class="pl-v">Vertex</span>{X: <span class="pl-c1">1</span>, <span class="pl-v">Y</span>: <span class="pl-c1">2</span>} <span class="pl-c"><span class="pl-c">//</span> Creates a struct by defining values with keys</span>
<span class="pl-k">var</span> <span class="pl-smi">v</span> = []<span class="pl-v">Vertex</span>{{<span class="pl-c1">1</span>,<span class="pl-c1">2</span>},{<span class="pl-c1">5</span>,<span class="pl-c1">2</span>},{<span class="pl-c1">5</span>,<span class="pl-c1">5</span>}} <span class="pl-c"><span class="pl-c">//</span> Initialize a slice of structs</span>

<span class="pl-c"><span class="pl-c">//</span> Accessing members</span>
v.<span class="pl-smi">X</span> = <span class="pl-c1">4</span>

<span class="pl-c"><span class="pl-c">//</span> You can declare methods on structs. The struct you want to declare the</span>
<span class="pl-c"><span class="pl-c">//</span> method on (the receiving type) comes between the the func keyword and</span>
<span class="pl-c"><span class="pl-c">//</span> the method name. The struct is copied on each method call(!)</span>
<span class="pl-k">func</span> <span class="pl-en">(<span class="pl-v">v</span> <span class="pl-v">Vertex</span>) <span class="pl-en">Abs</span></span>() <span class="pl-v">float64</span> {
    <span class="pl-k">return</span> math.<span class="pl-c1">Sqrt</span>(v.<span class="pl-smi">X</span>*v.<span class="pl-smi">X</span> + v.<span class="pl-smi">Y</span>*v.<span class="pl-smi">Y</span>)
}

<span class="pl-c"><span class="pl-c">//</span> Call method</span>
v.<span class="pl-c1">Abs</span>()

<span class="pl-c"><span class="pl-c">//</span> For mutating methods, you need to use a pointer (see below) to the Struct</span>
<span class="pl-c"><span class="pl-c">//</span> as the type. With this, the struct value is not copied for the method call.</span>
<span class="pl-k">func</span> <span class="pl-en">(<span class="pl-v">v</span> *<span class="pl-v">Vertex</span>) <span class="pl-en">add</span></span>(<span class="pl-v">n</span> <span class="pl-v">float64</span>) {
    v.<span class="pl-smi">X</span> += n
    v.<span class="pl-smi">Y</span> += n
}
</pre></div>
<p><strong>Anonymous structs:</strong>
Cheaper and safer than using <code>map[string]interface{}</code>.</p>
<div class="highlight highlight-source-go"><pre><span class="pl-smi">point</span> <span class="pl-k">:=</span> <span class="pl-k">struct</span> {
	<span class="pl-v">X</span>, <span class="pl-v">Y</span> <span class="pl-k">int</span>
}{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>}</pre></div>
<h2><a id="user-content-pointers" class="anchor" aria-hidden="true" href="#pointers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Pointers</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-smi">p</span> <span class="pl-k">:=</span> <span class="pl-v">Vertex</span>{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>}  <span class="pl-c"><span class="pl-c">//</span> p is a Vertex</span>
<span class="pl-smi">q</span> <span class="pl-k">:=</span> &amp;p            <span class="pl-c"><span class="pl-c">//</span> q is a pointer to a Vertex</span>
<span class="pl-smi">r</span> <span class="pl-k">:=</span> &amp;Vertex{<span class="pl-c1">1</span>, <span class="pl-c1">2</span>} <span class="pl-c"><span class="pl-c">//</span> r is also a pointer to a Vertex</span>

<span class="pl-c"><span class="pl-c">//</span> The type of a pointer to a Vertex is *Vertex</span>

<span class="pl-k">var</span> <span class="pl-smi">s</span> *Vertex = <span class="pl-c1">new</span>(Vertex) <span class="pl-c"><span class="pl-c">//</span> new creates a pointer to a new struct instance</span></pre></div>
<h2><a id="user-content-interfaces" class="anchor" aria-hidden="true" href="#interfaces"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Interfaces</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-c"><span class="pl-c">//</span> interface declaration</span>
<span class="pl-k">type</span> <span class="pl-v">Awesomizer</span> <span class="pl-k">interface</span> {
    <span class="pl-c1">Awesomize</span>() <span class="pl-k">string</span>
}

<span class="pl-c"><span class="pl-c">//</span> types do *not* declare to implement interfaces</span>
<span class="pl-k">type</span> <span class="pl-v">Foo</span> <span class="pl-k">struct</span> {}

<span class="pl-c"><span class="pl-c">//</span> instead, types implicitly satisfy an interface if they implement all required methods</span>
<span class="pl-k">func</span> <span class="pl-en">(<span class="pl-v">foo</span> <span class="pl-v">Foo</span>) <span class="pl-en">Awesomize</span></span>() <span class="pl-v">string</span> {
    <span class="pl-k">return</span> <span class="pl-s"><span class="pl-pds">"</span>Awesome!<span class="pl-pds">"</span></span>
}</pre></div>
<h2><a id="user-content-embedding" class="anchor" aria-hidden="true" href="#embedding"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Embedding</h2>
<p>There is no subclassing in Go. Instead, there is interface and struct embedding.</p>
<div class="highlight highlight-source-go"><pre><span class="pl-c"><span class="pl-c">//</span> ReadWriter implementations must satisfy both Reader and Writer</span>
<span class="pl-k">type</span> <span class="pl-v">ReadWriter</span> <span class="pl-k">interface</span> {
    <span class="pl-v">Reader</span>
    <span class="pl-v">Writer</span>
}

<span class="pl-c"><span class="pl-c">//</span> Server exposes all the methods that Logger has</span>
<span class="pl-k">type</span> <span class="pl-v">Server</span> <span class="pl-k">struct</span> {
    <span class="pl-v">Host</span> <span class="pl-k">string</span>
    <span class="pl-v">Port</span> <span class="pl-k">int</span>
    *log.<span class="pl-smi">Logger</span>
}

<span class="pl-c"><span class="pl-c">//</span> initialize the embedded type the usual way</span>
<span class="pl-smi">server</span> <span class="pl-k">:=</span> &amp;Server{<span class="pl-s"><span class="pl-pds">"</span>localhost<span class="pl-pds">"</span></span>, <span class="pl-c1">80</span>, log.<span class="pl-c1">New</span>(...)}

<span class="pl-c"><span class="pl-c">//</span> methods implemented on the embedded struct are passed through</span>
server.<span class="pl-c1">Log</span>(...) <span class="pl-c"><span class="pl-c">//</span> calls server.Logger.Log(...)</span>

<span class="pl-c"><span class="pl-c">//</span> the field name of the embedded type is its type name (in this case Logger)</span>
<span class="pl-k">var</span> <span class="pl-smi">logger</span> *log.<span class="pl-smi">Logger</span> = server.<span class="pl-smi">Logger</span></pre></div>
<h2><a id="user-content-errors" class="anchor" aria-hidden="true" href="#errors"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Errors</h2>
<p>There is no exception handling. Functions that might produce an error just declare an additional return value of type <code>Error</code>. This is the <code>Error</code> interface:</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">type</span> <span class="pl-k">error</span> <span class="pl-k">interface</span> {
    <span class="pl-c1">Error</span>() <span class="pl-k">string</span>
}</pre></div>
<p>A function that might return an error:</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">func</span> <span class="pl-en">doStuff</span>() (<span class="pl-v">int</span>, <span class="pl-v">error</span>) {
}

<span class="pl-k">func</span> <span class="pl-en">main</span>() {
    <span class="pl-smi">result</span>, <span class="pl-smi">err</span> <span class="pl-k">:=</span> <span class="pl-c1">doStuff</span>()
    <span class="pl-k">if</span> err != <span class="pl-c1">nil</span> {
        <span class="pl-c"><span class="pl-c">//</span> handle error</span>
    } <span class="pl-k">else</span> {
        <span class="pl-c"><span class="pl-c">//</span> all is good, use result</span>
    }
}</pre></div>
<h1><a id="user-content-concurrency" class="anchor" aria-hidden="true" href="#concurrency"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Concurrency</h1>
<h2><a id="user-content-goroutines" class="anchor" aria-hidden="true" href="#goroutines"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Goroutines</h2>
<p>Goroutines are lightweight threads (managed by Go, not OS threads). <code>go f(a, b)</code> starts a new goroutine which runs <code>f</code> (given <code>f</code> is a function).</p>
<div class="highlight highlight-source-go"><pre><span class="pl-c"><span class="pl-c">//</span> just a function (which can be later started as a goroutine)</span>
<span class="pl-k">func</span> <span class="pl-en">doStuff</span>(<span class="pl-v">s</span> <span class="pl-v">string</span>) {
}

<span class="pl-k">func</span> <span class="pl-en">main</span>() {
    <span class="pl-c"><span class="pl-c">//</span> using a named function in a goroutine</span>
    <span class="pl-k">go</span> <span class="pl-c1">doStuff</span>(<span class="pl-s"><span class="pl-pds">"</span>foobar<span class="pl-pds">"</span></span>)

    <span class="pl-c"><span class="pl-c">//</span> using an anonymous inner function in a goroutine</span>
    <span class="pl-k">go</span> <span class="pl-k">func</span> (x <span class="pl-k">int</span>) {
        <span class="pl-c"><span class="pl-c">//</span> function body goes here</span>
    }(<span class="pl-c1">42</span>)
}</pre></div>
<h2><a id="user-content-channels" class="anchor" aria-hidden="true" href="#channels"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Channels</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-smi">ch</span> <span class="pl-k">:=</span> <span class="pl-c1">make</span>(<span class="pl-k">chan</span> <span class="pl-k">int</span>) <span class="pl-c"><span class="pl-c">//</span> create a channel of type int</span>
ch <span class="pl-k">&lt;-</span> <span class="pl-c1">42</span>             <span class="pl-c"><span class="pl-c">//</span> Send a value to the channel ch.</span>
<span class="pl-smi">v</span> <span class="pl-k">:=</span> <span class="pl-k">&lt;-</span>ch            <span class="pl-c"><span class="pl-c">//</span> Receive a value from ch</span>

<span class="pl-c"><span class="pl-c">//</span> Non-buffered channels block. Read blocks when no value is available, write blocks until there is a read.</span>

<span class="pl-c"><span class="pl-c">//</span> Create a buffered channel. Writing to a buffered channels does not block if less than &lt;buffer size&gt; unread values have been written.</span>
<span class="pl-smi">ch</span> <span class="pl-k">:=</span> <span class="pl-c1">make</span>(<span class="pl-k">chan</span> <span class="pl-k">int</span>, <span class="pl-c1">100</span>)

<span class="pl-c1">close</span>(ch) <span class="pl-c"><span class="pl-c">//</span> closes the channel (only sender should close)</span>

<span class="pl-c"><span class="pl-c">//</span> read from channel and test if it has been closed</span>
<span class="pl-smi">v</span>, <span class="pl-smi">ok</span> <span class="pl-k">:=</span> <span class="pl-k">&lt;-</span>ch

<span class="pl-c"><span class="pl-c">//</span> if ok is false, channel has been closed</span>

<span class="pl-c"><span class="pl-c">//</span> Read from channel until it is closed</span>
<span class="pl-k">for</span> <span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-k">range</span> ch {
    fmt.<span class="pl-c1">Println</span>(i)
}

<span class="pl-c"><span class="pl-c">//</span> select blocks on multiple channel operations, if one unblocks, the corresponding case is executed</span>
<span class="pl-k">func</span> <span class="pl-en">doStuff</span>(<span class="pl-v">channelOut</span>, <span class="pl-v">channelIn</span> <span class="pl-v">chan</span> <span class="pl-v">int</span>) {
    <span class="pl-k">select</span> {
    <span class="pl-k">case</span> channelOut <span class="pl-k">&lt;-</span> <span class="pl-c1">42</span>:
        fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>We could write to channelOut!<span class="pl-pds">"</span></span>)
    <span class="pl-k">case</span> <span class="pl-smi">x</span> <span class="pl-k">:=</span> <span class="pl-k">&lt;-</span> channelIn:
        fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>We could read from channelIn<span class="pl-pds">"</span></span>)
    <span class="pl-k">case</span> <span class="pl-k">&lt;-</span>time.<span class="pl-c1">After</span>(time.<span class="pl-smi">Second</span> * <span class="pl-c1">1</span>):
        fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>timeout<span class="pl-pds">"</span></span>)
    }
}</pre></div>
<h3><a id="user-content-channel-axioms" class="anchor" aria-hidden="true" href="#channel-axioms"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Channel Axioms</h3>
<ul>
<li>
<p>A send to a nil channel blocks forever</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">c</span> <span class="pl-k">chan</span> <span class="pl-k">string</span>
c <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>Hello, World!<span class="pl-pds">"</span></span>
<span class="pl-c"><span class="pl-c">//</span> fatal error: all goroutines are asleep - deadlock!</span></pre></div>
</li>
<li>
<p>A receive from a nil channel blocks forever</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">c</span> <span class="pl-k">chan</span> <span class="pl-k">string</span>
fmt.<span class="pl-c1">Println</span>(<span class="pl-k">&lt;-</span>c)
<span class="pl-c"><span class="pl-c">//</span> fatal error: all goroutines are asleep - deadlock!</span></pre></div>
</li>
<li>
<p>A send to a closed channel panics</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">c</span> = <span class="pl-c1">make</span>(<span class="pl-k">chan</span> <span class="pl-k">string</span>, <span class="pl-c1">1</span>)
c <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>Hello, World!<span class="pl-pds">"</span></span>
<span class="pl-c1">close</span>(c)
c <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>Hello, Panic!<span class="pl-pds">"</span></span>
<span class="pl-c"><span class="pl-c">//</span> panic: send on closed channel</span></pre></div>
</li>
<li>
<p>A receive from a closed channel returns the zero value immediately</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">var</span> <span class="pl-smi">c</span> = <span class="pl-c1">make</span>(<span class="pl-k">chan</span> <span class="pl-k">int</span>, <span class="pl-c1">2</span>)
c <span class="pl-k">&lt;-</span> <span class="pl-c1">1</span>
c <span class="pl-k">&lt;-</span> <span class="pl-c1">2</span>
<span class="pl-c1">close</span>(c)
<span class="pl-k">for</span> <span class="pl-smi">i</span> <span class="pl-k">:=</span> <span class="pl-c1">0</span>; i &lt; <span class="pl-c1">3</span>; i++ {
    fmt.<span class="pl-c1">Printf</span>(<span class="pl-s"><span class="pl-pds">"</span><span class="pl-c1">%d</span> <span class="pl-pds">"</span></span>, <span class="pl-k">&lt;-</span>c)
}
<span class="pl-c"><span class="pl-c">//</span> 1 2 0</span></pre></div>
</li>
</ul>
<h2><a id="user-content-printing" class="anchor" aria-hidden="true" href="#printing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Printing</h2>
<div class="highlight highlight-source-go"><pre>fmt.<span class="pl-c1">Println</span>(<span class="pl-s"><span class="pl-pds">"</span>Hello, 你好, नमस्ते, Привет, ᎣᏏᏲ<span class="pl-pds">"</span></span>) <span class="pl-c"><span class="pl-c">//</span> basic print, plus newline</span>
<span class="pl-smi">p</span> <span class="pl-k">:=</span> <span class="pl-k">struct</span> { <span class="pl-v">X</span>, <span class="pl-v">Y</span> <span class="pl-k">int</span> }{ <span class="pl-c1">17</span>, <span class="pl-c1">2</span> }
fmt.<span class="pl-c1">Println</span>( <span class="pl-s"><span class="pl-pds">"</span>My point:<span class="pl-pds">"</span></span>, p, <span class="pl-s"><span class="pl-pds">"</span>x coord=<span class="pl-pds">"</span></span>, p.<span class="pl-smi">X</span> ) <span class="pl-c"><span class="pl-c">//</span> print structs, ints, etc</span>
<span class="pl-smi">s</span> <span class="pl-k">:=</span> fmt.<span class="pl-c1">Sprintln</span>( <span class="pl-s"><span class="pl-pds">"</span>My point:<span class="pl-pds">"</span></span>, p, <span class="pl-s"><span class="pl-pds">"</span>x coord=<span class="pl-pds">"</span></span>, p.<span class="pl-smi">X</span> ) <span class="pl-c"><span class="pl-c">//</span> print to string variable</span>

fmt.<span class="pl-c1">Printf</span>(<span class="pl-s"><span class="pl-pds">"</span><span class="pl-c1">%d</span> hex:<span class="pl-c1">%x</span> bin:<span class="pl-c1">%b</span> fp:<span class="pl-c1">%f</span> sci:<span class="pl-c1">%e</span><span class="pl-pds">"</span></span>,<span class="pl-c1">17</span>,<span class="pl-c1">17</span>,<span class="pl-c1">17</span>,<span class="pl-c1">17.0</span>,<span class="pl-c1">17.0</span>) <span class="pl-c"><span class="pl-c">//</span> c-ish format</span>
<span class="pl-smi">s2</span> <span class="pl-k">:=</span> fmt.<span class="pl-c1">Sprintf</span>( <span class="pl-s"><span class="pl-pds">"</span><span class="pl-c1">%d</span> <span class="pl-c1">%f</span><span class="pl-pds">"</span></span>, <span class="pl-c1">17</span>, <span class="pl-c1">17.0</span> ) <span class="pl-c"><span class="pl-c">//</span> formatted print to string variable</span>

<span class="pl-smi">hellomsg</span> <span class="pl-k">:=</span> <span class="pl-s"><span class="pl-pds">`</span></span>
<span class="pl-s"> "Hello" in Chinese is 你好 ('Ni Hao')</span>
<span class="pl-s"> "Hello" in Hindi is नमस्ते ('Namaste')</span>
<span class="pl-s"><span class="pl-pds">`</span></span> <span class="pl-c"><span class="pl-c">//</span> multi-line string literal, using back-tick at beginning and end</span></pre></div>
<h2><a id="user-content-reflection" class="anchor" aria-hidden="true" href="#reflection"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Reflection</h2>
<h3><a id="user-content-type-switch" class="anchor" aria-hidden="true" href="#type-switch"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Type Switch</h3>
<p>A type switch is like a regular switch statement, but the cases in a type switch specify types (not values), and those values are compared against the type of the value held by the given interface value.</p>
<div class="highlight highlight-source-go"><pre><span class="pl-k">func</span> <span class="pl-en">do</span>(<span class="pl-v">i</span> <span class="pl-v">interface</span>{}) {
	<span class="pl-k">switch</span> <span class="pl-smi">v</span> <span class="pl-k">:=</span> i.(<span class="pl-k">type</span>) {
	<span class="pl-k">case</span> <span class="pl-k">int</span>:
		fmt.<span class="pl-c1">Printf</span>(<span class="pl-s"><span class="pl-pds">"</span>Twice <span class="pl-c1">%v</span> is <span class="pl-c1">%v</span><span class="pl-cce">\n</span><span class="pl-pds">"</span></span>, v, v*<span class="pl-c1">2</span>)
	<span class="pl-k">case</span> <span class="pl-k">string</span>:
		fmt.<span class="pl-c1">Printf</span>(<span class="pl-s"><span class="pl-pds">"</span><span class="pl-c1">%q</span> is <span class="pl-c1">%v</span> bytes long<span class="pl-cce">\n</span><span class="pl-pds">"</span></span>, v, <span class="pl-c1">len</span>(v))
	<span class="pl-k">default</span>:
		fmt.<span class="pl-c1">Printf</span>(<span class="pl-s"><span class="pl-pds">"</span>I don't know about type <span class="pl-c1">%T</span>!<span class="pl-cce">\n</span><span class="pl-pds">"</span></span>, v)
	}
}

<span class="pl-k">func</span> <span class="pl-en">main</span>() {
	<span class="pl-c1">do</span>(<span class="pl-c1">21</span>)
	<span class="pl-c1">do</span>(<span class="pl-s"><span class="pl-pds">"</span>hello<span class="pl-pds">"</span></span>)
	<span class="pl-c1">do</span>(<span class="pl-c1">true</span>)
}</pre></div>
<h1><a id="user-content-snippets" class="anchor" aria-hidden="true" href="#snippets"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Snippets</h1>
<h2><a id="user-content-http-server" class="anchor" aria-hidden="true" href="#http-server"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>HTTP Server</h2>
<div class="highlight highlight-source-go"><pre><span class="pl-k">package</span> main

<span class="pl-k">import</span> (
    <span class="pl-s"><span class="pl-pds">"</span>fmt<span class="pl-pds">"</span></span>
    <span class="pl-s"><span class="pl-pds">"</span>net/http<span class="pl-pds">"</span></span>
)

<span class="pl-c"><span class="pl-c">//</span> define a type for the response</span>
<span class="pl-k">type</span> <span class="pl-v">Hello</span> <span class="pl-k">struct</span>{}

<span class="pl-c"><span class="pl-c">//</span> let that type implement the ServeHTTP method (defined in interface http.Handler)</span>
<span class="pl-k">func</span> <span class="pl-en">(<span class="pl-v">h</span> <span class="pl-v">Hello</span>) <span class="pl-en">ServeHTTP</span></span>(<span class="pl-v">w</span> <span class="pl-v">http</span>.<span class="pl-v">ResponseWriter</span>, <span class="pl-v">r</span> *<span class="pl-v">http</span>.<span class="pl-v">Request</span>) {
    fmt.<span class="pl-c1">Fprint</span>(w, <span class="pl-s"><span class="pl-pds">"</span>Hello!<span class="pl-pds">"</span></span>)
}

<span class="pl-k">func</span> <span class="pl-en">main</span>() {
    <span class="pl-k">var</span> <span class="pl-smi">h</span> Hello
    http.<span class="pl-c1">ListenAndServe</span>(<span class="pl-s"><span class="pl-pds">"</span>localhost:4000<span class="pl-pds">"</span></span>, h)
}

<span class="pl-c"><span class="pl-c">//</span> Here's the method signature of http.ServeHTTP:</span>
<span class="pl-c"><span class="pl-c">//</span> type Handler interface {</span>
<span class="pl-c"><span class="pl-c">//</span>     ServeHTTP(w http.ResponseWriter, r *http.Request)</span>
<span class="pl-c"><span class="pl-c">//</span> }</span></pre></div>
</article>
  </div>

    </div>

  

  <details class="details-reset details-overlay details-overlay-dark">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" action="" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
        <button type="submit" class="btn" data-close-dialog>Go</button>
</form>    </details-dialog>
  </details>



  </div>
</div>

    </main>
  </div>
  

  </div>

        
<div class="footer container-lg width-full p-responsive" role="contentinfo">
  <div class="position-relative d-flex flex-row-reverse flex-lg-row flex-wrap flex-lg-nowrap flex-justify-center flex-lg-justify-between pt-6 pb-2 mt-6 f6 text-gray border-top border-gray-light ">
    <ul class="list-style-none d-flex flex-wrap col-12 col-lg-5 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0">
      <li class="mr-3 mr-lg-0">&copy; 2019 <span title="0.24894s from unicorn-c4c56cdc5-vr7w8">GitHub</span>, Inc.</li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to terms, text:terms" href="https://github.com/site/terms">Terms</a></li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to privacy, text:privacy" href="https://github.com/site/privacy">Privacy</a></li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to security, text:security" href="https://github.com/security">Security</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://githubstatus.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a data-ga-click="Footer, go to help, text:help" href="https://help.github.com">Help</a></li>
    </ul>

    <a aria-label="Homepage" title="GitHub" class="footer-octicon d-none d-lg-block mx-lg-4" href="https://github.com">
      <svg height="24" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="24" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
   <ul class="list-style-none d-flex flex-wrap col-12 col-lg-5 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0">
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to contact, text:contact" href="https://github.com/contact">Contact GitHub</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://github.com/pricing" data-ga-click="Footer, go to Pricing, text:Pricing">Pricing</a></li>
      <li class="mr-3 mr-lg-0"><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li class="mr-3 mr-lg-0"><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://github.blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>

    </ul>
  </div>
  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 text-gray-light"></span>
  </div>
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
    You can’t perform that action at this time.
  </div>


    <script crossorigin="anonymous" integrity="sha512-BlCvumXWTvpASEdhCGiahDUDf7Bwb8QXA2XnnSnqJ9QafxcNcrNYUNYS2wXmd3nEpO//+zlZa9DSV9zmu5MqRg==" type="application/javascript" src="https://github.githubassets.com/assets/compat-bootstrap-90c0ace0.js"></script>
    <script crossorigin="anonymous" integrity="sha512-PFVbVSrMzusC1KLktzYYs16Ba4eiYgpG36jTWt0rbtvacsmX/QQFl+5ecqimZTvUKg8qbgeqGqVon2cTYh4Nvw==" type="application/javascript" src="https://github.githubassets.com/assets/frameworks-b1c626a0.js"></script>
    
    <script crossorigin="anonymous" async="async" integrity="sha512-w5sS5Hqgo7zwp/tCq1kOuj1QDDmqRusbQqY3s5+uPyJxu5nyEQrsUfgk04YKmG/li+8NlH9CazkCl+mRUn/4NQ==" type="application/javascript" src="https://github.githubassets.com/assets/github-bootstrap-927d0377.js"></script>
    
    
    
  <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner" hidden
    >
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark hx_rsm" open>
    <summary role="button" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast hx_rsm-dialog hx_rsm-modal">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

  <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box box-shadow-large" style="width:360px;">
  </div>
</div>

  <div aria-live="polite" class="js-global-screen-reader-notice sr-only"></div>

  </body>
</html>

