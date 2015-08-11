---
title: 'MS Word to DITA &#8211; Going From a Document Mindset to a Topic Mindset'
author: Sundar Nadimpalli
layout: post
permalink: /2015/03/01/ms-word-to-dita-going-from-a-document-mindset-to-a-topic-mindset/
categories:
  - Technical Writing
---
Going from using a software like MS Word to using DITA for documentation is somewhat like going from manually machining a metal rod on a lathe to programmatic machining using a CNC machine. DITA lets you incorporate intelligence into your documentation. Let&#8217;s look at the first stage of the planning that needs to be done to adopt DITA.

<!--more-->

## The Challenge

One of the first challenges that you will face going from MS Word to DITA is thinking in terms of Topics instead of Documents. One of the first rules of DITA content creation is that a topic should be as short as possible and it should contain only one type of content. For example, lets say that you are creating documentation for cleaning a car. Then the topic of your documentation where you talk about cleaning the tyres of the car should not include steps on how to clean the under body of the car. The tire cleaning topic should only be about cleaning tires.

You need to take this topic mind set all the way. To explore this further, let us look the user manuals that a hypothetical car cleaning service. Let us also imagine that they service 25 different types of cars and car cleaning process for each car (although similar to a large extent) is a little different. To further our cause, I am going to further imagine that they have 25 user manuals in MS Word format. The service manager now wants use DITA to manage and produce the documentation.

The imaginary manager of the car cleaning service has handed you one of the user manuals and the table of contents of the user manual looks as shown below.

**Table of Contents**

  1. Introduction &#8211; The importance of keeping the car clean
  2. Cleaning the Exterior 
      1. Washing the Body
      2. Cleaning the Windows
      3. Washing the Tires
      4. Washing the Under body
      5. Waxing and Polishing
  3. Cleaning the Interiors 
      1. Cleaning the Carpet
      2. Cleaning the Seats
      3. Cleaning the Dashboard
      4. Cleaning the Doors
      5. Cleaning the Glass Surfaces
      6. Cleaning the Boot
  4. Keeping the Car Clean

Now let us look at how you can take this user manual to plan your DITA conversion. The first step would be to create a table like one shown below. The table of contents of your user manual document will be your guide.

### Table of Contents to a DITA Map

<table dir="ltr" border="1" cellspacing="0" cellpadding="0">
  <colgroup> <col width="29" /> <col width="319" /> <col width="230" /> <col width="100" /></colgroup> <tr>
    <td>
      <strong>#</strong>
    </td>
    
    <td>
      <strong>Original User Manual TOC</strong>
    </td>
    
    <td>
      <strong>DITA Map</strong>
    </td>
    
    <td>
      <strong>Topic Type</strong>
    </td>
  </tr>
  
  <tr>
    <td>
      1
    </td>
    
    <td>
      Introduction &#8211; The importance of keeping the car clean
    </td>
    
    <td>
      Introduction to Keeping Your Car Clean
    </td>
    
    <td>
      Concept
    </td>
  </tr>
  
  <tr>
    <td>
      2
    </td>
    
    <td>
      Cleaning the Exterior
    </td>
    
    <td>
      Cleaning the Exterior
    </td>
    
    <td>
      Concept
    </td>
  </tr>
  
  <tr>
    <td>
      2.1
    </td>
    
    <td>
      Washing the Body
    </td>
    
    <td>
      &#8212; Washing the Outer Body
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      2.2
    </td>
    
    <td>
      Cleaning the Windows
    </td>
    
    <td>
      &#8212; Cleaning the Windows
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      2.3
    </td>
    
    <td>
      Washing the Tires
    </td>
    
    <td>
      &#8212; Washing the Tires
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      2.4
    </td>
    
    <td>
      Washing the Under body
    </td>
    
    <td>
      &#8212; Washing the Under Body
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      2.5
    </td>
    
    <td>
      Waxing and Polishing
    </td>
    
    <td>
      &#8212; Waxing the Polishing
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      3
    </td>
    
    <td>
      Cleaning the Interiors
    </td>
    
    <td>
      Cleaning the Interiors
    </td>
    
    <td>
      Concept
    </td>
  </tr>
  
  <tr>
    <td>
      3.1
    </td>
    
    <td>
      Cleaning the Carpet
    </td>
    
    <td>
      &#8212; Cleaning the Carpet
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      3.2
    </td>
    
    <td>
      Cleaning the Seats
    </td>
    
    <td>
      &#8212; Cleaning the Seats
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      3.3
    </td>
    
    <td>
      Cleaning the Dashboard
    </td>
    
    <td>
      &#8212; Cleaning the Dashboard
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      3.4
    </td>
    
    <td>
      Cleaning the Doors
    </td>
    
    <td>
      &#8212; Cleaning the Doors
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      3.5
    </td>
    
    <td>
      Cleaning the Glass Surfaces
    </td>
    
    <td>
      &#8212; Cleaning the Glass Surfaces
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      3.6
    </td>
    
    <td>
      Cleaning the Boot
    </td>
    
    <td>
      &#8212; Cleaning the Boot
    </td>
    
    <td>
      Task
    </td>
  </tr>
  
  <tr>
    <td>
      4
    </td>
    
    <td>
      Keeping the Car Clean
    </td>
    
    <td>
      Keeping the Car Clean
    </td>
    
    <td>
      Concept
    </td>
  </tr>
</table>

### How to Classify the Topics

To understand how to classify the topics in valid DITA topic types, you need to understand the various DITA topic types. The table like one shown above is possible if you audit each of the topic in your user manual and try to classify the topic as any one of the following types:

  1. Concept &#8211; <a title="DITA Concepts" href="http://docs.oasis-open.org/dita/v1.0/archspec/dita_spec_22_info_concepts.html" target="_blank">Click here to know more about DITA Concepts</a>
  2. Task &#8211; <a title="DITA Tasks" href="http://docs.oasis-open.org/dita/v1.0/archspec/dita_spec_22_info_tasks.html" target="_blank">Click here to know more about DITA Tasks</a>
  3. Reference &#8211; <a title="DITA Reference Topic" href="http://docs.oasis-open.org/dita/v1.0/archspec/dita_spec_22_info_refs.html" target="_blank">Click here to know more about DITA References</a>

Once you have classified the topics in the user manual it becomes very easy to make the classification. In the next post I will go into further detail of taking an example topic of the existing user manual and converting that to a DITA topic.
