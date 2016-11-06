---
title: Working with Flex 2 on Mac OS X
author: Rob Bevan
layout: post
permalink: /2005/10/23/working-with-flex-2-on-mac-os-x/
categories:
  - Software
---
(<span style="color: red;">Note:</span> this post was originally written on release of the Flex 2 alpha. I&#8217;ve since updated it for the Flex 2 beta.)

Macromedia recently announced [Macromedia Labs][1] and the availability of the Flex 2 product line alpha, which includes a new Eclipse-based IDE and a new high performance client runtime (Flash Player 8.5) alongside the development framework. Unfortunately, for now, development on the Mac is not supported and Macromedia only provide an installer for Flex Builder 2, the Flex Framework 2, Flex samples and command line tools for Windows.

So I set about trying to discover, if [as with the 1.0 release,][2] I could get the framework at least to run on OS X: and the short answer is yes, it&#8217;s relatively simple.

First of <span class="hilite">all</span> you need to extract both the framework and the player from the [Download for Windows][3]. To do this, just unzip the relevant components from the .exe file. Assuming you&#8217;ve already downloaded FlexBuilder2\_Beta1\_Install.exe to your desktop, [this script][4] does exactly this and then copies the &#8216;frameworks&#8217; and &#8216;lib&#8217; directories to a flex2 directory in /Library <strike>and the Install Flash Player 8.5 OSX.dmg to your desktop</strike>. (Or you can obviously just run the installer on Windows and copy across the relevant files.)

Once you&#8217;ve got the framework installed, you can use mxmlc &#8211; the (Java) Macromedia Flex Compiler &#8211; from the command line or better still with [Ant][5]. Here&#8217;s a version of the &#8216;Hello World&#8217; example Flex project from Macromedia&#8217;s Quick-start tutorials book with the simplest possible Ant build file: just [download][6] and run &#8216;ant&#8217; (defaults to the &#8216;build&#8217; task) in the Quickstart directory, and &#8211; assuming you&#8217;ve already installed the player &#8211; then open QuickStart.html. You should see the movie initialise and the words &#8220;Welcome to Flex&#8221; appear.

(I had no luck at <span class="hilite">all</span> getting the IDE work, I did try extracting Flex Builder 2&#8242;s &#8216;features&#8217; and &#8216;plugins&#8217; directories and copying the contents of these to my Eclipse installation. Although I was then able to create a new Flex project, I wasn&#8217;t able to start the MXML editor which failed with a NullPointerException.)

<div class="update">
  <p>
    Update: in case you missed the original Flex 2 <a href="http://www.macromedia.com/macromedia/proom/pr/2005/announcing_flex2.html">announcement</a> and were wondering why you&#8217;d bother investing any time in an expensive enterprise-only technology, Macromedia also announced a new (very welcome) licensing model for Flex:
  </p>
  
  <p>
    &#8220;Macromedia is also introducing a new tiered licensing model to bring the power of Flex development within reach of every professional application developer, while also offering value-added capabilities that scale to meet the needs of the most sophisticated enterprise projects. Flex Builder 2 will be sold for less than $1000 per developer and will include the ability to develop, compile, and deploy Flex applications that connect to XML and SOAP web services with no additional charges or server licensing required. Flex Enterprise Services 2 will be licensed on a per CPU, per project, and enterprise license basis to offer the development efficiency, performance, advanced integration capabilities, and testing support that advanced applications will require.&#8221;
  </p>
</div>

<div class="update">
  <p>
    Update: Mike Chambers has a round up of resources for <a href="http://weblogs.macromedia.com/mesh/archives/2006/01/resources_for_c.cfm">Compiling ActionScript 3 and MXML from the command line</a>.
  </p>
</div>

<p class="technorati-tags">
  (Technorati tags: <a href="http://technorati.com/tag/flash" rel="tag">flash</a> | <a href="http://technorati.com/tag/flex-2" rel="tag">flex-2</a> | <a href="http://technorati.com/tag/os-x" rel="tag">os-x</a>)
</p>

 [1]: http://labs.macromedia.com/
 [2]: http://robbevan.com/blog/2004/04/04/running-macromedia-flex-with-jboss-on-mac-os-x-server/
 [3]: http://labs.macromedia.com/downloads/
 [4]: http://www.bigbold.com/snippets/posts/show/1619
 [5]: http://ant.apache.org
 [6]: http://robbevan.com/blog/wp-content/uploads/working_with_flex_2_beta_1_on_mac_os_x.zip