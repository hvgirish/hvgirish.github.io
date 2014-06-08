---
layout: post
title:  "When to DevOps?"
date:   2014-05-27 18:37:00
categories: definitions
---

In the previous post we saw what the fuss was all about DevOps. In this post, we will look at when an organisation/project must adopt DevOps practises and what kind of orgs/projects it suits. And what the criterias are to make the decision.

So `The Management`&trade; hears a buzzword called DevOps and wants to adopt it instantly. There's no turning back now (you know, your designation and team names are changed, the updated Org Charts are out, complete with the hoopla that ensues). All you have in your control is to evaluate what you can adopt and when (the timeline).

Traditional Opeartions teams are _usually_ manually driven. When there's a change requested, it is done manually on the servers that need the change, after communicating to all stakeholders. The team is not open to automating what they do repeatedly, either because there is no enough time or because they aren't trained for it.

Operations teams would rather install the heavy-duty nonsense systems/network operations management software from multi-billion dollar enterprises that either change the way the team works by enforcing a different process/workflow or integrates with the existing heavy-duty crap they already have. These software either dont work for the infrastructure that the organisation already has or is too inflexible for design changes. Very few teams focus only on the _really mundane_ tasks and get them automated, if they ever do.

Development teams, however, are more `agile`. OpenSource software proliferation and awareness has made most developers adopt and practise lean processes using popular tools and techniques, sometimes, just for the heck of it and sometimes, more reasonably/responsibly. In anycase, they have the unit tests, they do CI, they refactor vehemently, avoid repetitions (you get the drift). They want to automate all the shtuff! Thats where we have the problem. Because operations teams are very rarely in the same context as Dev teams.

```Automation is a crucial piece. If the organisation focus is not on investing in people who want to learn automation and start writing scripts/programs for infrastructure, then DevOps adoption is going to be so much more harder```

Its easier when DevOps adoption goes hand-in-hand with adopting Agile methodologies. It would make it easier for a developer and an operations engineer to think in terms of tasks and progress over a shorter period of time. Incremental changes to infrastrucure and application code would get along seamlessly.

DevOps mindset also suits SaaS and PaaS software delivery models. That is because of the control and flexibility the operations team have in releasing and managing the product along with the speed at which the development teams can churn out features. This does not mean companies with standalone products cannot adopt devops mindset. Its just that getting people on the same page becomes harder when your install base is practically every other laptop in the world. Your install scripts (unless designed properly) bloat up to handle every corner case possible.

Opensource software adoption and use goes a long way. Many are written well, using most of the devopsy techniques and are easy to understand and maintain, in general, yielding faster/better results. Companies that have a love-hate relationship with opensource software will find it hard to buy these techniques.

DevOps way of building software also needs to be internalised quite early in the product design and implementation. Once you have something working, the temptation to have workarounds and `hacks` for building and deploying the product out-weigh the **right way** of doing things. And it is both developers and the operations engineers who take the worst hit. Nobody likes to be called at 3am to be looking at a service that refuses to start after a config change when there is no centralised logging or visibility of what the config change was and whether it was deployed to all servers or not or even then, whether the service was really reloaded or not.

With this context set, we will look at how exactly DevOps mindset makes a difference in regular everyday tasks by looking at examples.
