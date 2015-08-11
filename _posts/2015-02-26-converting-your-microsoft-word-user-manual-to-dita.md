---
title: Converting A Microsoft Word User Manual to DITA Format
author: Sundar Nadimpalli
layout: post
permalink: /2015/02/26/converting-your-microsoft-word-user-manual-to-dita/
geo_public:
  - 0
dsq_thread_id:
  - 3827783271
categories:
  - Technical Writing
---
One of my first assignments in my new job was to convert the existing user manuals that were created using MS Word to a more modern documentation framework. The company wide decision was to move to DITA. In this article I will write about how I converted a MS Word user manual to DITA.

<!--more-->

## The oXygenXML Editor

The tool was chosen for the DITA implementation at our company was the <a title="The oXygen XML Editor" href="http://oxygenxml.com/" target="_blank">oXygenXML Editor</a>. It has excellent support for authoring content in the DITA format and makes the job of the content author super easy. One of the most valuable features that I found to be useful was that the XML editor checks if the content that I type is valid DITA as and when I try to add a new element into a topic.

I find the editor really instructive and I feel that I am learning how to create valid DITA topics as the editor constantly checks and corrects me.

## The DITA Way

Although I do not want to talk much about DITA itself in this post, writing technical content in DITA meant that, as an author I had to start thinking differently than when I was writing the user manual in MS Word.

The DITA content types that I used so far are:

  1. Task Topics
  2. Concept Topics
  3. Reference Topics

To get a crash course in DITA <a title="Useful DITA Introductory Tutorial" href="http://www.xmlmind.com/tutorials/DITA/" target="_blank">this nifty tutorial</a> written by the kind folks at XMLMind is a must read.

### The Steps to go from MS Word to DITA

The top level steps that I went through when converting the MS Word User manual to DITA was something like this:

  1. Review the table of contents of the MS Word user manual
  2. Create an excel file to help with planning the MS Word TOC to Dita Map conversion
  3. Go over each item in the MS Word TOC and try to classify the topic to its most appropriate DITA topic type equivalent
  4. Look at the contents of each topic in the MS Word file and decide if its needs to be split up into smaller topics
  5. Decide the file name for each of the topics that need to be created
  6. Start moving the content from the MS Word file to individual topic dita files

The above steps are of course in their over simplified form. Each of the step listed above needs further explanation. I will try to expand each of them in posts that will follow in the coming days.
