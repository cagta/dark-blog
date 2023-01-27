---
title: localhost while vpn is on?
description: "damn corporate policies" 
category: essays
tags: technical english
permalink: /blog/localhost-while-vpn-is-on
date: 2020-04-10 10:31
syntax: true
---
as a developer, i'm always looking for ways to improve my development environment. to be honest, i'm too lazy to repeat silly manual operations again and again. and today i'm gonna share one of my way of doing that.

since i'm a corporate guy, while i'm away from my office i'm using our corporate vpn. why i'm repeating this corporate thing again and again because when you are in such a big company you mostly have very limited space to change things in your favor. for example, in this case, i have to divide my internet traffic into two separate parts. the traffic that needs to be going on a vpn and the traffic that needs to be going on my localhost.

i need that because, in default, if you are using vpn it means the local network was changing. so if you had a virtual machine which is running on your local pc like mine, it will become inaccessible since your local network was changed.

i overcame this situation by using the port forwarding feature of the oracle virtualbox. with the help of that now i can access all of my services which is actually on my virtual machine.

even the one image will tell you the story which can be seen below. go to your network settings of you virtual machine then add one nat interface to your machine and at the advance option of this interface add some port mappings like below. and here we go. now we can access the webserver which is being served over port 80 of the virtual machine and accessible on port 8080 of my host. 

<img src="/static/images/posts/2020-04-10-ayvmwctv-oracle-virtual-box.png">