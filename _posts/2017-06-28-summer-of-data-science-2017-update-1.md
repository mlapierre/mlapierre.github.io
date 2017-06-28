---
layout: single
title:  "Summer of Data Science 2017 - Update 1"
date:   2017-06-28 17:11:12 -0400
categories: data-science
tags: SoDS17
---
My dataset/corpus is coming together. 

It was relatively easy to create a set of text files from the articles I'd saved to Evernote. It's taking more time to collect a set of articles that I didn't find interesting enough to save. I'll make that easier in the future by automatically saving *all* the articles that pass through my feed reader, but for now I'm grabbing copies from CommonCrawl. This saves me the trouble of crawling dozens of different websites, but I still have to search the CommonCrawl index to find articles among everything else in the index from each site. 

I created a list of all the site I'd saved at least one article from, then I downloaded the CommonCrawl index records for each site from the last two years. Next I filtered the records to include only pages that were likely to be articles (e.g., no 'about' or 'contact' pages, etc.). I took a random sample of up to 100 of the records remaining for each site and downloaded the WARC records, and then extracted and saved each article's text. I'll make all the code available once I've polished it a little.

The next step will be to explore the dataset a little before diving into topic analysis.