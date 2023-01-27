---
title: seiatc - how i'm using python?
description: "python rocks!" 
category: essays
tags: technical english
permalink: /blog/seiatc-how-i-m-using-python
date: 2021-06-23 10:31
syntax: true
---
welcome to my second post of software engineer in a telecommunication company series. if you didn’t check the first post yet. you can read it from this [link](/blog/software-engineer-in-a-telecommunication-company/).

python is one the oldest member of my skill set. as you may already know that i’m not a tool fanatic. i don’t see any value on this. programming languages are the tools that we are using to solve our real life problems. we may like one of them more than others but benefiting from all is better. after this explanation you may see my stand clearly. i love python, but this doesn’t stop me from seeing its disadvantages as well as advantages.

according to [official site](https://www.python.org/about/) _“python is a programming language that lets you work more quickly and integrate your systems more effectively.”_ i think it provides what it’s proposing. if we were talking more technically, its one of the interpreted languages. which means your code will be read and interpreted line by line.

i don’t want to dig into discussions like _‘is python fast enough ?’_, _‘why you should use python for this and not to use for that ?’_ instead i would like to mention that why it’s a good choice for our case.

<strong>easy to learn</strong>

python has a very simple syntax. you may argue with me about indentations however if you check the numbers of python projects, we can say that there is lots of people who already adopted it. by the way, those people have very different backgrounds from high school teachers to bioinformatic engineers.

<strong>collection of libraries</strong>

as a software engineer, i like to see what stays under the hood. however when its come to building a complex systems, i don’t prefer to invent the wheel while there is a stable, accessible solution. python has lots of libraries which ensure these expectations. let’s take a look what i’m using frequently.

if you are dealing with network equipment, you need to deal with lots of ip math. **ipaddress** and **netaddr** libraries are very useful for these kind of operations. if it’s just a simple operations like checking ip version, ip validation etc. , i prefer built-in ipaddress library. but for more complex operations like assigning an ip from a specific subnet, checking subnet size according to topology etc. , netaddr is my choose. but instead of being a built-in library, netaddr is a bsd licensed third-party library that widely used in network address manipulation.

ip manipulations are only the beginning of our journey. accessing network equipment and gathering information about this device as important as preparing an ip pooling without overlap. there is several different network equipment on the market. even if i’m working for one of the vendors, i need to know that how to access other vendors’ devices and what kind of information is available on these devices for me. that information is critique especially on migrating from a third-party network.

for that information, i need to access these devices then process the available data. **netmiko/paramiko** libraries are very common within our team. to be honest, i don’t even care to compare them. i just used whichever presented in the project that i contribute. since i only use them to establish ssh connections, i don’t think it’ll make any difference :)

when it’s come to gather and process these kind of data **textfsm** is my best friend. according to it’s documentation textfsm is a `python module which implements a template based state machine for parsing semi-formatted text.` thanks to it we can easily parse and get related information from several different devices.

<strong>wide application range</strong>

with the help of diverse libraries and core feature of the language you can use python with a variety of the fields from embedding applications to web applications. thanks to that we had a chance to build both web applications and simple terminal applications with the same team without shifting over technologies.

after all, i’m happy with python for now. let me know what’s your experience.