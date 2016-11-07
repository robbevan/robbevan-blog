---
title: Running Macromedia Flex with JBoss on Mac OS X Server
author: Rob Bevan
layout: post
permalink: /2004/04/04/running-macromedia-flex-with-jboss-on-mac-os-x-server/
categories:
  - Software
---
Although one of the early [Flex][1] beta installers for Linux also worked on Mac OS X, this is no longer true for the 1.0 release version. However, this doesn&#8217;t mean it can&#8217;t be installed. <span class="hilite">All</span> you need to do is extract the WAR files from the installer: `unzip -d flex flex-10-lin.bin` (extracting the contents of the archive to a new directory &#8216;flex&#8217; in the working directory). These will be in the dist directory at `flex/R_/dist`. Each WAR file is a separate, stand-alone application, and should be installed on the server with its own directory structure and context. For example, to install the samples, extract the contents of this archive to JBoss&#8217;s `deploy` directory e.g. `unzip -d /Library/JBoss/3.2/deploy/samples.war flex/R_/dist/samples.war.zip`, then wait about a minute for the JBoss engine to do its thing before accessing the application: `http://localhost:8080/samples`.

<strike>The [Flex trial][2] CD can be ordered from the Macromedia store for $8.99.</strike>

<div class="update">
  Update: the 1.5 installer now works on Mac OS X (although Mac OS X is still an unsupported platform). The 1.5 trial is now <a href="http://www.macromedia.com/software/flex/trial/">available for download</a>. I tried the IBM AIX version, as this was the smallest download. It&#8217;s not possible to change the default install directory (<code>/Macromedia/Flex</code>), but otherwise the installer works as expected.
</div>

 [1]: http://www.macromedia.com/devnet/flex/
 [2]: http://www.macromedia.com/software/flex/trial/