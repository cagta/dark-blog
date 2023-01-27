---
title: story of the my weekend project!
description: "so small for world, a lot for me" 
category: essays
tags: technical english
permalink: /blog/story-of-the-my-weekend-project
date: 2020-04-18 10:31
syntax: true
---
this weekend, i coded two simple python tool for myself. it feels great when you accomplished this kind of things. i don't even remember when was the last time that i built this kind of satisfying side project. i think it is satisfying because it solves one of my problem.

i really like to ready articles about anything that triggers my curiosity. it includes bunch of things like history, psychology, business, economy, applied science and of cource computer science. so i have to reach out lot's of different resource to gather these article. they are mostly online web articles but sometimes i'm downloading pdfs, docs, epubs etc.

at the beginning, i was reading all of them on my computer and on my phone. i have to admit that it was mostly on my phone because i can carry it everywhere with me easily so that i can read it on bus, while waiting some friends etc. which means i can turn almost all of my idle time into productive entertainment.

however after a while my eyes start to complain. since i'm computer engineer, i'm always looking at screens when i added this idle times my eyes were really tired. after these complaints i discovered the e-ink technology and amazon kindle. e-ink is a amazing technology. for more detail about the technology, you should check [this](https://www.youtube.com/watch?v=oqu1--azm7u) but short explaination is you can read your digital contents on a digital screen which looks almost like real paper.

after all, why i'm telling these? this post should be about a tool that i coded right? here's the deal. everytime that i want to pick some cool contents to read on my toy, i have go and find that contents for me. basically, i have great list of rss on my feedly for person or focused online news platform. and i'm also hanging aroud bunch of other sites to pick articles.

it's as consuming as reading. so want to cut that time to increase my reading time. i was start to think about it, since i'm developing some automation tools for others for money. i think i can use that logic to gain my time. it's leads me to [gather-my-news](https://github.com/cagta/gather-my-news).

i started very small. this simple script go [dev.to](https://dev.to) -which is one of my most visited site on daily scrapping- and gathers most popular articles on weekly basis.
it prepares a list of the articles for me so that i can check them easily without any distraction. i can easily check their title's to detirmine if there is anythin catchy or not and their systatics(likes and comments). it really like this for two reason. first, i'm directly accessing audince approved articles. second, i can see what i need without dealing with fancy side bars and graphics which are mostly nothing but distracting.

i'm planning to add [world economic forum's reports](https://www.weforum.org/reports) and [world turkish business council's reports](http://www.dtik.org.tr/yayinlar) to my script as soon as possible.

i would like to stop writing now for this post with giving technologies that i used as conclusion. i know i only tell you about one simple tool maybe i can mention the other on my next post.

ingredients of my tool:

- [python](https://www.python.org/) as base programming language
- [beautifulsoup](https://www.crummy.com/software/beautifulsoup/) for proccesing html
- [urllib](https://docs.python.org/3/library/urllib.html) for handling url