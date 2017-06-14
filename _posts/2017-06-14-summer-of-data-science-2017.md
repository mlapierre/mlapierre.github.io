---
layout: single
title:  "Summer of Data Science 2017"
date:   2017-06-14 17:45:17 -0400
categories: data-science
tags: SoDS17
---
Goal: To launch<sup id="fnr1"><a href="#fn1">*</a></sup> my learn'ed system for coping with the information firehose
-----
I heard about the [Summer of Data Science 2017](https://www.becomingadatascientist.com/2017/05/29/summer-of-data-science-2017/) recently and decided to join in. I like learning by doing so I chose a personal project as the focus of my efforts to enhance my data science skills.

For the past *forever* I've been stopping and starting one side-project in particular. It's a system that searches and filters many sources of information to provide me with articles/papers/web pages relevant to my interests. It will use NLP and machine learning to model my interests and to predict whether I'm likely to find a new article worthwhile. Like a recommender system but just for me, because I'm selfish. Something like [Winds](https://winds.getstream.io/). The idea is to collect all the articles I read/skim/ignore via an RSS reader, and tag those I find interesting. And to build up a Zotero collection of papers of several degrees of quality and interest. Those tagged and untagged articles and papers will comprise my datasets. There is a lot more to this project, but that's the core of it.

My first (mis)step was to begin building an RSS reader than could automatically gather data on my reading habits that I could use to infer interest based on my behaviour; whether I clicked a link to the full article, how long I spent reading an article, whether I shared it, etc. Recently I decided that was not the best use of my time, as it would be much easier to start with explicitly tagged articles--I can start gathering those without creating a new tool. So I'm doing that by saving interesting articles to Evernote. Today I have just under 900. I can use CommonCrawl to get all the articles I *didn't* find interesting on the relevant sites (i.e., the articles that would have appeared in my RSS reader, but which I didn't save).

There are many things I'll need to do before I'm done, but all of those depend on having a dataset I can analyse. So my next step will be to turn those Evernote notes and other articles into a dataset suitable for consumption by NLP tools. Given the tools available for transforming text-based datasets from one format to another, I'm not going to spend much time choosing a particular format. I'll start with a set of plain-text copies of each article and associated metadata, and take it from there.

I've been less consistent in gathering research papers. I've been saving the best papers I've stumbled across, but I could do much better by approaching it as a research project, i.e., do a literature review. That's a huge task so I'll focus on analysing web articles first.

<p style="font-size:12px" id="fn1"><a href="#fnr1">*</a>I was going to write "complete" but really, it'll always be changing and will probably never be complete. But ready for automated capture and analysis? Sure, I can make that happen.</p>
