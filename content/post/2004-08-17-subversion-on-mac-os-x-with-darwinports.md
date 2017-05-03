---
title: Subversion on Mac OS X with DarwinPorts
date: "2004-08-16T23:41:17Z"
author: Rob Bevan
permalink: /2004/08/17/subversion-on-mac-os-x-with-darwinports/
categories:
  - Software
---
I wish I&#8217;d had the benefit of [this article][1] a few months back when I was setting up my [Subversion][2] server. Although the [svn documentation][3] is excellent, it&#8217;s good to see a Mac OS X specific tutorial.

Installing Subversion (plus dependencies) using [DarwinPorts][4] is really simple: just cd to your darwinports/dports/ directory and type `sudo port install subversion +mod_dav_svn`. Instructions on how to install DarwinPorts are [here][5].

I put together a [Subversion startup item][6] (installed into /Library/StartUpItems/), although really this is just an Apache2 startup item, but I called it Subversion since that&#8217;s <span class="hilite">all</span> I&#8217;m using Apache2 for. The script assumes you&#8217;ve installed Apache2 in /opt/local/apache2, and requires SVNSERVER=-YES- to be added to /etc/hostconfig.

<div class="update">
  <p>
    Update: Apple has now has a useful article <a href="http://developer.apple.com/tools/subversionxcode.html">Getting Control with Subversion and Xcode</a> detailing how to compile Subversion from source for use with the version of Apache2 shipped with Mac OS X Server, as well as how to install <a href="http://websvn.tigris.org/">WebSVN</a>, which offers as web-based &#8220;view onto your subversion repositories that&#8217;s been designed to reflect the Subversion methodology&#8221;. Although I&#8217;m not sure why an article about Subversion suggests downloading WebSVN rather than checking it out from the svn repository:
  </p>

  <p>
    <code>svn co http://guest:guest@websvn.tigris.org/svn/websvn/tags/1.61/ websvn</code></div> <p class="technorati-tags">
      (Technorati tags: <a href="http://technorati.com/tag/subversion" rel="tag">subversion</a> | <a href="http://technorati.com/tag/darwinports" rel="tag">darwinports</a>)
    </p>

 [1]: http://www.oreillynet.com/pub/au/1943
 [2]: http://subversion.tigris.org/
 [3]: http://svnbook.red-bean.com/svnbook/
 [4]: http://darwinports.opendarwin.org/
 [5]: http://darwinports.opendarwin.org/docs/ch01s03.html
 [6]: http://robbevan.com/blog/wp-content/uploads/subversion_startupitem.pkg.zip
