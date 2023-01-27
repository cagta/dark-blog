---
layout: post
title: git tag; lightweight or annotated?
description: "use git" 
category: essays
tags: technical english
permalink: /blog/git-tag-lightweight-or-annotated
date: 2021-06-28 10:31
syntax: true
---
>_<strong>tldr;</strong> use annotated tags that contain tagger name, email, date, and message. in that way, you can isolate taggers from commit authors. you can see who tagged which commit. otherwise, you would have just the author of the commit. you can also secure them with a gpg sign. on the other hand, lightweight tags are just simple pointers. you may prefer to use them privately to put a pinpoint on your commit history._

git has two different tag types: lightweight and annotated. at first sight, you may think there is no problem using them interchangeably. however, the git commands like 'git describe' take annotated tags by default. of course, you can use related flags and bypass this behavior like 'git describe - tags'. however, let me show you why you may prefer annotated tags over the lightweight ones. the most common scenario for using tags is releasing a new version.

consider this scenario, you are a newbie in a team of 10 developers. somehow you need to investigate one of the older versions of your project because of a problem at production. and you saw that this code should not ship in the first place. at that time, you may want to be sure about your judgment. so who should you talk to? this is where things get interesting. if the release tag is lightweight, you will see something like this.

```bash
$ git show v1.4
commit ca82a6dff817ec66f44342007202690a58967412
author: cagatay tanyildiz <cagta@mail.com>
date:   fri 25 21:52:11 2021 -0300
   
   change version number
```

which is quite unclear who made that tagging? yes, you can still see the author of a specific commit. but do you remember all of the auditors of your codes? i don't think so. so the first advantage of annotated tags is detailed information which is absent in lightweight tags and isolating the tagger of the commit from the author of the commit. in that way, you can see who made this commit and who tagged it as a valid production commit.

let's think of another way. you built a jenkins pipeline that takes all the tags from your repository and changes production code each time it detects a release tag. if you built your system on top of lightweight tags, you should think twice. how you are traceback your release even if you are not sure who approved it? again, author/auditor isolation is needed.

lastly, you may have a customer who wants to ensure that they pull in a verified set of changes onto their platforms. in that case, you need to gpg sign each of your release tags. this is only applicable to annotated tags because of their information storing capacity. more specifically, they contain the tagger name, email, date, and the message. also, they can be signed with gpg. check 'whodunnit for paranoid people' section of this article for detail. an annotated tag will look like this.

```bash
$ git show v1.2
tag v1.2
tagger: cagatay tanyildiz <cagta@mail.com>
date:   fri 25 22:12:11 2021 -0300

version 1.2
commit ca82a6dff817ec66f44342007202690a58967412
author: cagatay tanyildiz <cagta@mail.com>
date:   fri 25 21:52:11 2021 -0300

    update location list
...
```

in conclusion, you should use annotated tags by default which have more detail than lightweight tags, even if you are not sharing them with others. otherwise, you can neither see the tagger nor sign it when you need it.