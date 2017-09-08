---
layout: single
title:  "Summer of Data Science 2017 - Final Update"
categories: data-science
tags: SoDS17, classification, topic-analysis
---
Ok, so it's not summer any more. My defence is that I did this work during summer but I'm only *writing* about it now.

To recap, I'd been working on a smart filter; a system to predict articles I'd like based on articles I'd previously found interesting. I'm calling it my rss-thingy / smart filter / information assistant<sup id="fnr1"><a href="#fn1">1</a></sup>. I'm tempted to call it "theia", short for the information assistant, and a play on "the AI", but it sounds too much like a siri rip-off.

Aaaanyway, I'd collected 660 interesting articles and 801 that I didn't find interesting--fewer than expected, but I had to get rid of some that were too short or weren't articles (e.g., lists of links, or github repositories). There was also a bit of manual work to make sure none of the 'misses' were actually 'hits'. I.e., I didn't want interesting articles to turn up as misses, so I skimmed through all the misses to make sure they weren't coincidentally interesting (there were a few). The hits and misses then went into separate folders, ready to be loaded by scikit-learn.

I used scikit-learn to vectorise the documents as a tf-idf matrix, and then trained a linear support vector machine and a naive bayes classifier. Both showed reasonable precision and recall upon my first attempt, but tests on new articles showed that the classifier tended to categorise articles as misses, even if I did find them interesting. This is not particularly surprising; most articles I'm exposed to are not particularly interesting, and such simple models trained on a relatively small dataset are unlikely to be exceptionally accurate in identifying them. I spent a little time tuning the models without getting very far and decided to take a step sideways before going further.

Eventually I'll want to group potentially interesting articles, so I wrote up a quick topic analysis of the articles I liked, comparing non-negative matrix factorization with latent dirichlet allocation. They did a reasonable job of identifying common themes, including brain research, health research, science, technology, politics, testing, and, of course, data science.

You can see the code for [this informal experiment](https://github.com/mlapierre/SoDS17) on github.

In my next experiment (now, not SoDS18!) I plan to refine the predictions by paying more attention to cleaning and pre-processing the data. And I need to brush up on tuning these models. I'll also use the trained models to make ranked predictions rather than simple binary classifications. The dataset will be a little bigger now at around 800 interesting articles, and a few thousand not-so-interesting.

<p style="font-size:12px" id="fn1"><a href="#fnr1">1.</a> Given all the trouble I have naming things, I'm really glad I haven't had to do any cache-invalidation yet.</p>
