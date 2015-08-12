---
title: Modifying the Default Footer of DITA Web Help Output from oXygen XML Editor
author: Sundar Nadimpalli
layout: post
permalink: /2015/03/03/modifying-the-default-footer-of-dita-web-help-output-from-oxygen-xml-editor/
categories:
  - Technical Writing
---
Modifying the default footer that oXygen XML Editor writes out to the DITA Webhelp transformation is done through a parameter called **WEBHELP\_FOOTER\_FILE**. The steps below describes the process to modify the footer.

<!--more-->

The default footer looks something like the image below.

<img class="alignnone size-full wp-image-14" src="https://s3.amazonaws.com/sundar-website-assets/images/dita_default_footer.png?fit=419%2C55" alt="The default footer written out by DITA. " data-recalc-dims="1" />

You can change it to anything you want. The steps to the same are given below.

  1. Create a new well formed XHTML file containing the HTML content that you want displayed in the footer. For example: <pre class="brush: xml; title: ; notranslate" title="">&lt;div&gt;
  &lt;p&gt;
    A Packaged Solution Offering by Your Company Name.
 &lt;/p&gt;
&lt;/div&gt;
</pre>

  2. Save this file on your computer as an html/xhtml file and copy the full file name along with its path.
  3. Open the file dita2webhelp.xsl in oXygen XML Editor or a text editor like Notepad++ or Sublime Text, the file is usually located in this folder **&#8211; C:\Program Files\Oxygen XML Editor 16\frameworks\dita\DITA-OT\plugins\com.oxygenxml.webhelp\xsl\dita\dita2webhelp.xsl** (on a windows machine).
  4. On line 23, edit the parameter **WEBHELP\_FOOTER\_FILE** and specify the full path and file name that you copied to the clipboard in step 2
  5. Save the **dita2webhelp.xsl** file.
  6. Open oXygen XML Editor validate your DITA content and run the Webhelp transformation to regenerate the Webhelp output.

**Note:** Do not include any HTML symbols like 

<pre class="brush: plain; title: ; notranslate" title="">&copy;</pre>

etc in the footer content. Including this in the footer content might cause the footer to not render properly in the webhelp output.

You should now be able to see the new footer in the webhelp output.

<img class="alignnone size-full wp-image-44" src="https://s3.amazonaws.com/sundar-website-assets/images/new_modified_footer1.png?fit=313%2C87" alt="New Custom Footer" data-recalc-dims="1" />

&nbsp;
