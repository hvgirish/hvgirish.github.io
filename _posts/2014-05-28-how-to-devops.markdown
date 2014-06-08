---
layout: post
title:  "How to DevOps?"
date:   2014-05-28 19:45:00
categories: techniques
---

Like I said in earlier posts, DevOps is about prioritising Dev and Ops tasks equally. Its mostly about recognising that, as soon as you have something to deliver (however little that may be), you will have to also maintain it, operationally, especially through the development phase where your product is going to morph into a monster. You want to be able to quickly do this so that you can get to the features instead of wasting time setting up infra over and over again. Hence its in your best interest to build the product in a way that it makes it easy for the Ops folks. What better way than just involving the Ops folks and getting them to automate _all_ the shtuff? (well, almost _all_ :P)

With that out there, lets identify the _basic_ `non-functional`* requirements that any product needs to have in _this_ order.

* A mechanism to unit test developer changes with quicker feedback loops (this includes ops codebase changes too)  
* Be able to run as non-root user  
* Configurable (levels and destinations) Logging to gain visibility into what the product is doing (for times when a regular stack trace isn't enough)  
* Init scripts (LSB or systemd, pick your poison) to reliably start, stop and print status of services  
* Externalise the configuration  
* Depending on the language and frameworks selected, maybe something that `builds` the product binaries  
* Some automated, scalable and revertable deployment mechanism  
* Atleast one QA, Staging and Production environments each, with builds promoted from one to another  

* `Non-functional` is a funny word some non-technical people use for DevOps'y tasks. For example, people think externalising configuration is non-functional. People think capacity planning and deployment are non-fucntional. In the SaaS world, the distinction is very hard to make. If the response times for your app is unreasonable, it doesn't matter if the code works on your dev box. Part of adopting the DevOps mindset is to understand that there _are no_ 'non-functional' requirements.

TDD helps, a _lot_, wherever feasible. Write tests first. Let it go red. Write the feature. Make it go green. Iterate. This _usually_ works. Except that most of the code that you actually write, for operations, cannot have tests since the tools aren't available. Or aren't relevant, in case of the new breed of config management systems (I am looking at you, Puppet/Chef/Vagrant/docker).

Personally, the TDD I follow, when I write shell and perl or rarely, ruby scripts comes down to these steps.  

* Open up a terminal  
* Enter your favorite unix command to fetch the output you want to go ahead with the task  
* Insert and wrap command around backticks or a system() call  
* Iterate till script completion  

Sounds good? Most of my scripts, are `test complete`, by the time I develop. With chef and puppet, the workflow changes a bit, but is quick enough when the associated tools are also setup.

We'll see all of this in future posts when we work on real examples. Keep the basic requirements in mind. You will be very lucky if you can get all of this _before_ you even showcase the first few features to your customer. Lets work towards enabling that.
