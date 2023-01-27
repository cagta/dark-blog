---
title: seiatc - how i'm using git?
description: "i can not praise git enough" 
category: essays
tags: technical english
permalink: /blog/seiatc-how-i-m-using-git
date: 2021-07-24 10:31
syntax: true
---
welcome to my third post of software engineer in a telecommunication company series. if you didn’t check the previous posts yet, check the links below. 

* [software engineer in a telecommunication company](/blog/software-engineer-in-a-telecommunication-company/)
* [seiatc - how i'm using python?](/blog/seiatc-how-i-m-using-python/)

my main objective is experimenting with ideas with git. anytime i want, i can easily create a branch and work on my new ideas without breaking the existing codebase. i prefer to use `git checkout -b newbranchname`. it is like a combination of `git branch newbranchname` and `git checkout newbranchname`. after that, i directly jump on the code and try my ideas.

sometimes i come up with another solution while coding the other one. at that time, i am using `git stash` to remove all unstaged changes. this command lets me start over and save the current changes. i am using this store as a shelf of possible solutions. `-m` flag let you write notes about your stash. if you want to remember what is going on with that version of the changes, i strongly suggest using it. but let's be honest, most of the time, we are skipping that :) at least, git keeps track of our stashing with a number. keep in mind, it is working like a stack. the first stashed changes place at the bottom of the list.

let's dig into another use case. in an ideal world, we should have a development and commit plan before starting to code. i will be honest with you. mostly it is not the case. the problem looks too easy to solve then you start typing. just a couple of minutes later, you notice your assumption is wrong. after that minute, you start coming back and forth while trying to enhance your solution. you can guess how this will affect your commit history.

`git rebase -i` is probably my favorite command. you can divide your commits into smaller chunks, can edit their messages, and can rewrite your whole commit history. i like this feature and widely use it. however, i am only using it if the branch that i am working on is not public. when you use rebase, it will change your commits' hashes. if you are working on a public one, this means disaster for your colleagues. so be careful about it.

before closing, i would like to mention some valuable resources that can enhance your git knowledge.

* [simplify writing code with deliberate commits](https://youtu.be/mE8DZUfhdm4)
    * it suggests 5 practical habits which will make your commits more deliberate.

* [a branch in time](https://tekin.co.uk/2019/02/a-talk-about-revision-histories)
    * a talk about the revision history.

* [how github uses github to build github](https://youtu.be/qyz3jkOBbQY)
    * it is probably the oldest resource that i am sharing with you. but there are still valuable and valid bits of advice in it. on the other hand, do not let the title misleads you. you will find valuable information about git.

* [git tip: committing with verbose mode](https://tekin.co.uk/2020/03/git-commit-verbose-mode)
    * after i discover verbose mode, i never looked back.

`self marketing warning!! the following article is mine. so i can not be objective about it. :)`
* [git tag; lightweight or annotated?](/blog/git-tag-lightweight-or-annotated/)
    * let's you decide which type of tag is more useful for your case.