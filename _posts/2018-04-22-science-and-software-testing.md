---
layout: single
title:  "Science and software testing"
date:   2018-04-22 19:31:00 -0400
tags: testing science
---
Software testing, particularly manual software testing, is sometimes thought of as nothing more than following a script to confirm that the software does what it was designed to do. From that perspective, testing might seem like a boring and relatively mindless task. And to be honest, that *is* [the traditional view](https://qacomplete.com/resources/articles/what-is-manual-testing/#manual_testing_as_script_following) of testing as part of the Waterfall method of software development in large organisations. Division of labour meant that there were some people who did nothing but follow scripts someone else had written, and report bugs that someone else would fix.

Science, on the other hand, is undeniably interesting and challenging. So if you share the impression that software testing is boring, you might be suprised to know that I find both engaging and worth spending my time and effort on<sup id="fnr1"><a href="#fn1">1</a></sup>. Having worked as a software tester, and having studied a scientific field (cognitive science), I've noticed some similarities that help explain why I'm drawn to both persuits despite their apparent lack of similarity.

[Science can be defined as](https://en.oxforddictionaries.com/definition/science):

> "The intellectual and practical activity encompassing the systematic study of the structure and behaviour of the physical and natural world through observation and experiment."

That doesn't seem to describe following testing scripts at all. Even if you swap "the physical and natural world" for "the software under test", and even if you include the task of writing scripts. But if you consider the entire process of software testing you'll see similarities emerge. For one thing, test scripts have to be written based on something, and in today's world of agile software development, than something is usually *not* requirements handed down from designers, but rather requirements explored, developed, and refined iteratively. [Observation and experiment are a big part of that iterative process](https://qacomplete.com/resources/articles/what-is-manual-testing/#manual_testing_as_script_following). This is especially the case when working on existing software that doesn't have good documentation&mdash;how else could you figure out how the software works except through observation and experiment? Even if you have access to the code, it's unlikely you could read the code and know exactly how the software will behave. And there isn't always someone else around to ask.

The reality of software testing is a lot more than following a script. A more complete [definition of testing](http://www.satisfice.com/blog/archives/856) is that:

> "Testing is the process of evaluating a product by learning about it through exploration and experimentation, which includes to some degree: questioning, study, modeling, observation, inference, etc." 

When defined that way, it's much clearer how testing and science are similar. Questioning, study, modeling, observation, and inference are all core aspects of science and testing. 

In testing, we question whether the software does what we expect it to do. We question whether it does what customers want it to do and in the way they want. We question whether a code change has unintended effects. We study how the software behaves under various conditions. We construct models of how we believe the software performs, even if they're only mental models. We observe how the software responds to input. And ultimately we make inferences about the quality of the software.

Another similarity between science and software testing is that neither process truly has an end. There is always more to discover through science, even at the end of a project that has produced significant insights. And there is always more to learn about any but the simplest software. In the case of science and testing, it's not meaningful to think of the entire process as having a goal, but it is necessary to define a reasonable milestone as the completion of a project. We don't finish testing when there are no bugs, because that will never happen, but we can consider testing complete when the software behaves well under a reasonable range of scenarios.

Science is often described as trying to prove things<sup id="fnr2"><a href="#fn2">2</a></sup>. That is not the aim of science, nor is it how science works. [Science is, in part, a way of trying to better understand the world](https://undsci.berkeley.edu/article/0_0_0/whatisscience_04). And science is the knowledge produced by that process. The scientific method involves making a hypothesis and then gathering evidence and analysing data to draw conclusions about whether the hypothesis is supported. It's possible to find evidence that rules out a hypothesis, but it's not possible find evidence that a particular hypothesis is *the only* explanation for the data. This is because other hypotheses might explain that evidence just as well, including hypotheses that no-one has come up with yet. But after carefully analysing the results of many experiments a clearer understanding can begin to emerge (in the form of a theory). In that way you can think of science as showing what doesn't work until there's a reasonably solid explanation left. It's not about being right; it's about being less wrong. 

Similarly, testing isn't about proving that the software is bug free; it's about providing evidence that you can use the software without any significant issues, so that what's left is reasonably solid. It's also not about proving that the software does exactly what the customer wants, but it is about helping to iteratively improve the customer's satisfaction with the software. This is an important part of software testing that's sometimes forgotten&mdash;the aim isn't solely to find bugs, but also to find unexpected, unusual, or confusing behaviour.

On the other hand, there are plenty of ways in which science and testing are different. But I'll leave that for another post. 
 
<p style="font-size:12px" id="fn1"><a href="#fnr1">1.</a> Not so much manual testing specifically, but a comprehensive approach to testing that includes exploratory testing and automation.
<p style="font-size:12px" id="fn2"><a href="#fnr2">2.</a> Do a search for "<a href="https://www.google.com/search?q=science+proves">science proves</a>". It's enough to make a scientist or philosopher or mathematician cry.