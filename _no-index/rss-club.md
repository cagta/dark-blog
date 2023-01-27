---
title: rss club
description: 'this is my “secret” page only for people on my rss list'
permalink: /rss-club
nav: main
---

welcome to my rss only section, where i keep more personal content away from search engines and the public face of this site. 

this is the last frontier of the old and internet: no tracking or algorithmic filter bubbles.

check out other bloggers in [dave rupert’s rss club](https://daverupert.com/2018/01/welcome-to-rss-club/). 


## rss only posts 

{% for post in site.categories.rss-club %}

{% include blog-listing.html %}

{% endfor %}
