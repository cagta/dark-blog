---
title: my first firefox extension - tab2hyperlink
description: "love shortcuts" 
category: essays
tags: technical english
permalink: /blog/my-first-firefox-extension
date: 2020-06-22 10:31
syntax: true
---
i don't even remember when i was started to use [firefox](https://www.mozilla.org/en-us/firefox/new/) as my default web browser. i liked it because it's open source and easily configurable according to my privacy needs. today's internet world is build on tracking and analysing tools which i prefer to leave myself out of it. this concerns can be a topic of another post but you can check [prism-break](https://prism-break.org/en/) for further details. today's topic is my first firefox extension: tab2hyperlinklist. 

why i coded a firefox browser? as some you already know i'm a kindle lover. thanks to amazon [send2kindle](https://www.amazon.com/gp/sendtokindle/) i'm reading almost every article on my feed from kindle. i'm putting too much effort to find valuable contents for me each week. basically, i'm using [feedly](https://feedly.com/) to subscribe rss feeds, using good old email subscription to gather news from both paid or free qualified sources like [bbc](http://pages.emails.bbc.com/subscribe/), [hbr turkey](https://hbrturkiye.com/), [apisecuritio](https://apisecurity.io/) and lastly using my simple [script]((https://github.com/cagta/gather-my-news)) to gather weekly news from varios sources. thanks to [dev.to](https://dev.to) i have to update the last one since they do not want bots. while reading all of these articles i'm using clippings function to analyze all of those and if it seems interesting enough to me i'm sharing them with you on the homepage of this blog.

so i have a bookmark directory which is called "blog" to collect all of the valuable resources for sharing with you. even most of them came from kindle sometimes i'm adding stuff from custom resources like youtube etc. at the end of the week i have to open each link from this directory and convert them to something like this:

```html
     <li><span>22 june 2020</span> &raquo; <a href="https://duckduckgo.com/">duckduckgo</a></li>
```

so i can share each item with you. these days, it started to seems like a nightmare to me after gathering bunch of stuff i have to put one more manual boring step to make them ready to publish. i decided to write an extension to automate it. what i though is since i'm opening those links for further analysis after gathering clippings from my kindle, i could use that as a start point. 

first i read this very helpful and simple [article](https://developer.mozilla.org/en-us/docs/mozilla/add-ons/webextensions/your_first_webextension) to understand the structure of the firefox extension. after that i though i can use [tabs api](https://developer.mozilla.org/en-us/docs/mozilla/add-ons/webextensions/api/tabs) to get my needs which is the url of the open tabs and their title. while structuring it i noticed that i have to pick a logo to publish my tiny extension. thanks to [cc license](https://creativecommons.org/licenses/) and the creator of the icon, i pick a little [armchair](https://www.iconarchive.com/show/free-flat-sample-icons-by-thesquid.ink/armchair-icon.html) which has a strong connection with my armchair fetish =) i love reading stuffs on that. after that i build this tiny little [thing](https://github.com/cagta/tab2hyperlink) which i hope it will make difference for me.

if you want to install that you can check it from [here](https://addons.mozilla.org/en-us/firefox/addon/tab2hyperlinklist/?src=search).