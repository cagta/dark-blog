---
title: summary of devops readings
description: "devs love ops" 
category: essays
tags: technical english
permalink: /blog/summary-of-devops-readings
date: 2021-01-03 10:31
syntax: true
---
some of you may already know, while i'm trying learn something new, i like to dig in multiple resources to see different aspects of it and prepare a summary from all of them. with that way i believe i'm learning way better and sharing this knowledge makes me feel like, i'm giving back to community.

today, we are gonna talk about devops. before writing this summary devops was a frequently heard trending topic for me. i thought it was just a new field at software world. i was seeing vacancies which are titled as devops engineer alongside with several discussions about devops like tool comparisons, role/responsibility sharing etc. besides that, i was feeling like i'm just seeing the results instead of the needs and the starting point of this trendy topic. we are talking about devops since late 2008. there are several definitions of devops, i will try to give the most convincing one for me. 

let's start with dev of devops. we can say that every thing we do for building our softwares is dev side of devops; designing, coding, testing etc. after creating softwares we should run them without any trouble in a designated place with acceptable performance. everything we do to ensure that can be seen as ops part of devops; monitoring, incident management, maintainence, performance evaluation etc. another definition can be this: dev is the people who are involved with building software and ops is the operations needed while building, testing, maintainining/providing services. 

all of these explanations are both wrong and right. they are right because all of these are some part of devops. but they are also wrong because devops means unification of the concepts not separation of them. "devops is defined by people building software and how they work together, not simply by what’s in their toolchain." [[1]](https://github.blog/2020-10-07-devops-definition/)

so why do we need to unify these concepts? because, we want to ship our softwares faster than ever without sacrificing stability and security. thing about google, facebook, github or any other company you see as a pioneer of the software world. the conditions and the expectations of the world is changing rapidly. no one tolerate 1 hour denial of service anymore. in critical system, even minutes can be seem unacceptable. this is not new. but the thing is world expecting you to deliver that quality within days or months not within years. while you are providing security and stability, there is always a new feature to be discovered or introduced. pioneers want to be either innovators or early adopters [[2]](https://en.wikipedia.org/wiki/technology_adoption_life_cycle). even being an early majority may be considered as failure.

<img src="https://upload.wikimedia.org/wikipedia/commons/4/45/DiffusionOfInnovation.png">

while we are facing such a big demand there is no way except unifying all the stakeholders of the process. for me this is what devops is. all the things which let us work more closely than before to produce stable, secure and efficient softwares. all the stakeholders should be aligned and be aware of each other's way of work.

<img src="/static/images/posts/2021-01-03-devops.png">

i took the figure above from andrew clay's presentation [[3]](https://youtu.be/idcnynmpb44?t=1919) i believe it's is great in terms of showing the whole concept of devops. 

finally, after giving brief information about the devops. i encourage you to dig in the details of resources that i follow while writing this post.

**resources**
- [what is devops? a guide to common methods and misconceptions](https://github.blog/2020-10-07-devops-definition/)
- [getting started with devops automation](https://github.blog/2020-10-29-getting-started-with-devops-automation/)
- [the evolving role of operations in devops](https://github.blog/2020-12-03-the-evolving-role-of-operations-in-devops/)
- andrew clay shafer's [closing keynote - elemental devops](https://www.youtube.com/watch?v=idcnynmpb44&list=pltmfdka8k73yuhx2tutvnayp6xjxo-4c9) at devopsdays istanbul 2018 
- andrew clay shafer's [closing keynote](https://www.youtube.com/watch?v=k2zplnijpbi) at devopsdays istanbul 2019 

**references**
- [1] [https://github.blog/2020-10-07-devops-definition/](https://github.blog/2020-10-07-devops-definition/)
- [2] [https://en.wikipedia.org/wiki/technology_adoption_life_cycle](https://en.wikipedia.org/wiki/technology_adoption_life_cycle)
- [3] [https://youtu.be/idcnynmpb44?t=1919](https://youtu.be/idcnynmpb44?t=1919)