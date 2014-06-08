---
layout: post
title:  "What is DevOps?!"
date:   2014-05-25 14:54:00
categories: definitions
---

So, what is _DevOps_? You will find many websites saying a lot of things. Wikipedia basically scares you with a lot of fancy terminology. You may feel like its not a `real` role. Something that involves _Software Development_, _Release Management_, _Quality Assurance_, _Security_, _Reliability_, _Deployment/Maintenance_, _Audit/Monitoring_, _Performance Measurement and Tuning_ and _Budgeting/Cost Analysis_ cannot be `real` afterall. Check out this image from wikipedia.

<pre id="img" align="center"><img src="http://upload.wikimedia.org/wikipedia/commons/b/b5/Devops.svg"></pre>

Thats totally unreal, you say?

Its not as bad as you might think. A _DevOps_ Engineer/Consultant is not expected to be an expert following all the above domains for advances in technology _all_ the time. Although, s(he) is expected to be `aware of trends` in most of these domains.

In a SaaS/PaaS based product (typically in a startup or a small sized company - because it _generally_ doesn't take much to run a website) where you have a couple of people responsible for IT Infrastructure Operations, you end-up making most of the critical architectural decisions for the product during initial design and development of the product. Most of those architectural decisions are about how 'the product' would use the infrastructure and whether thats optimal, how cost effective it is, how the business would plan to sustain it, how the Operations team would manage/maintain/scale the product effectively while driving continuous development and release of the product.

Answers to these questions would imply use of specific tools and technologies to achieve what are called the _Operational_ aspects of the product. Examples include Centralised/Indexed/Searcheable logfiles management, Measuring and Monitoring core operational and performance indicators, automating the Build and Deploy process, detecting auto-scaling needs and responding with Infrastructure and Service provisioning, responding to issues raised by customers (internal and external) etc.

In a medium/large sized company with an already exising product/solution set (once again, SaaS/PaaS based), together with an existing operations team with traditional ops mindset, it is just about trying to figure out how you can help reduce/optimise release cycles and keep the collaboration between development and operations teams transparent, seamless and less intrusive to each others activities, all the while trying hard to move them from the traditional ops to the devops way, so as to reap the benefits of lean processes.

So, the right answer is _It depends_. There is no clear definition for the 'DevOps' role. I actually dont even think its a 'role' with specific skillset. (And yet I call myself a DevOps consultant! :P You will see why in a moment)

```DevOps is a mindset. Every Developer, QA Engineer, Ops Engineers, BA, PM and even the client, when DevOps'ified, would just start considering operational aspects of the product along with the feature set that the client intends to have developed, in the planning, design and implementation phases.```

In the chart above, imagine TechOps and Software Development in one huge circle called DevOps. Thats the DevOps 'role' I am talking about, if there is one. (I would still keep QA out since the idealogy behind QA applies to both Ops and Dev world)

In traditional software development, a product team would just focus on hacking away features for the product and ensuring that it is defect-free, while the operations team would only focus on deploying the product to production and managing/maintaining it. When the team gets DevOps'ified, everybody stars prioritising the operational aspects `on-par` with the core feature set. That way, you get the best of both worlds, with lesser friction among developers and operations engineers. What you develop as a team becomes `operational` very quick and easy. Developers and operations engineers become equally capable of bringing in changes to the entire eco-system of creating the product and successfully running it, fixing it and iterating over releases, using familiar processes and tools.

Well, that was, sort of, the `idea`. And ideas are hard to sell. So, different organisations and products, based on their experience and awareness have varied adoption rates of this idea. And based on that, if you were a so-called DevOps guy/gal, you would experience the entire spectrum of emotions from boredom to elation in your work environment. And the DevOps adoption is so varied that we have ended up making it a role so we can cater to all sorts of people and organisations in the industry.

If you fancy a comic definition, heres one : 
```DevOps is what came out of frustrated developers who were too agonised not being able to talk to operations engineers to get the job done.```

We will look at _[When to DevOps](http://hvgirish.github.io/definitions/2014/05/28/when-to-devops.html)_ in an upcoming post and then get down to 'how to devops' with real examples aka `stuff that _really_ matter`.
