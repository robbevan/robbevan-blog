---
title: AppleJacked!
date: "2005-11-01T23:46:36Z"
author: Rob Bevan
permalink: /2005/11/01/applejacked/
categories:
  - Software
---
For some reason, my PowerBook decided not to recognise me this morning and wouldn&#8217;t allow me to log in. Eventually, I figured out I could reset my (corrupt) account&#8217;s password from the login window using my &#8216;master password&#8217;, but then I wasn&#8217;t able to start up to anything other than a blue screen. (Coincidentally, I&#8217;d earlier read that one of[ Mac OS X 10.4.3&#8242;s][1] fixes &#8211; released today &#8211; addressed (an unrelated) [issue][2] in which high ASCII characters in a password could lead to a blue screen at startup, or prevent log in.) Previously I&#8217;d been able to fix this kind of problem by booting into single user mode and renaming Preferences and Caches folders as detailed in [this Apple tech note][3], but today this didn&#8217;t help. I finally figured out I simply needed to reset my account&#8217;s password back to match that of my home folder&#8217;s FileVault disk image.

Apart from providing myself with a reminder of what to do next time, this post is by way of introduction to [AppleJack][4], an excellent utility I came across today that enables you to run a set of tasks in sequence to repair your disk, repair permissions, validate the system&#8217;s preference files and get rid of possibly corrupted cache files, <span class="hilite">all</span> without loading the GUI.

 [1]: http://docs.info.apple.com/article.html?artnum=301984
 [2]: http://docs.info.apple.com/article.html?artnum=302231
 [3]: http://docs.info.apple.com/article.html?artnum=106464
 [4]: http://applejack.sourceforge.net/
