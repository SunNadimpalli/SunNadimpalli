---
title: How To Embed a HTML5 Video in a DITA Topic for the Webhelp Output
author: Sundar Nadimpalli
layout: post
permalink: /2015/03/06/embed-html5-video-in-a-dita-topic-for-webhelp-output/
categories:
  - Technical Writing
---
If you want to embed a HTML5 Video in a DITA topic for the Webhelp transformation when using oXygenXML Editor, the steps below might be useful to you.

<!--more-->

## Steps to Configure the Object Element for Video Output

  1. Open the topic where you want to insert a video in the **oXygenXML Editor**.
  2. Click the location where you want to insert the video.
  3. Add a new **Object** element to the topic.
  4. Edit the Attributes for this Object element and a value of &#8220;video&#8221; to the **outputclass** attribute.  
    <img class="alignnone size-full wp-image-28" src="https://s3.amazonaws.com/sundar-website-assets/images/video-object-attribute-outputclass.png?fit=250%2C225" alt="The videoclass Attribute for an Object element" data-recalc-dims="1" /></p> 
  5. Add a new param child element to this Object.  
    Enter the name of the param as **src**.
  6. In the value for this param, enter the path to the MP4 video file. (If you want to embed a youtube video, you can enter the URL to the youtube video here.)
  7. To specify a fixed height to the video add a new param with the name **width **and enter the required width as the value for the param. You can even enter 100% for the height or width params and the same will reflect in the output. 
    <img class="alignnone size-full wp-image-29" src="https://s3.amazonaws.com/sundar-website-assets/images/insert-html5-video-object.png?fit=660%2C357" alt="DITA Object for Inserting a Video Element in a Topic" data-recalc-dims="1" /> </li> 
    
      * <span style="line-height: 1.5;">Generate the DITA Webhelp output to see the video in the help output.</span></ol> 
    
    &nbsp;
