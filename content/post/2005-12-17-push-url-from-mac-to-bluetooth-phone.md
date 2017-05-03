---
title: Push url from Mac to bluetooth phone
date: "2005-12-17T06:28:29Z"
author: Rob Bevan
permalink: /2005/12/17/push-url-from-mac-to-bluetooth-phone/
categories:
  - Mobile
  - Software
---
Something that seems unnecessarily cumbersome to me is getting a url from my Mac to my phone (a [Nokia 6630][1]). So I knocked up a simple solution using [QuickSilver][2] and Framework Labs&#8217; [Bluetooth Object Push Automator Action][3] stuck together with a little AppleScript.

After you&#8217;ve installed the action, create an [Automator][4] workflow using the Push File to Bluetooth Device action, configure it for your device (assuming you&#8217;ve already set up your phone for use with your Mac using the Bluetooth Setup Assistant) and save this to your desktop as an application named Push2Phone. (Anything you drop on this app will now get pushed to your phone.)

<img style="padding-bottom: 10px;"  src="http://robbevan.com/blog/wp-content/themes/robbevan/images/posts/bluetooth-push-automator-action.png" alt="" />

Then copy [this AppleScript][5] for QuickSilver to `~/Library/Application Support/QuickSilver/Actions` and **be sure to modify the tmp\_file\_path and app_path properties in the script for your environment**.

<img style="padding: 0 10px 16px 0;"  src="http://robbevan.com/blog/wp-content/themes/robbevan/images/posts/push2phone-6630-screenshot.png" alt="" />

Now you should be able to select a url &#8211; like this:

<strong style="padding: 2px; border: 1px solid #ccc;">http://m.gmail.com</strong>

Google&#8217;s new [mobile version of Gmail][6] &#8211; and in Safari hit Cmd-% to send this to QuickSilver (in Firefox you&#8217;ll need to cut and paste) and then type &#8216;pu&#8217; or similar to forward it to your phone.

<div class="update">
  Update: Interesting sidenote: seems you can use Google&#8217;s mobile gateway to convert your site (and any site you link to) to WML simply by pre-pending http://www.google.com/gwt/n?u= to your url:</p> <p>
    <strong style="padding: 2px; border: 1px solid #ccc;">http://www.google.com/gwt/n?u=http://blog.robbevan.com&_gwt_noimg=1</strong>
  </p>

  <p>
    (via <a href="http://muness.blogspot.com/2005/12/google-wml-gateway.html">Mundane Essays</a>) </div> <p>
      See also <a href="http://www.impossibilities.com/blog/entry_blog-196.php">Robert Hall&#8217;s post</a> on how to use the Bluetooth Object Push Automator Action to enhance Flash Lite development.
    </p>

    <p>
      Now <span class="hilite">all</span> I need to do is to figure out how to make Opera the default browser on my phone. Anyone know if this is possible?
    </p>

    <p class="technorati-tags">
      (<img style="float: none; padding: 2px 2px 0 2px;"  src="http://robbevan.com/blog/wp-content/themes/robbevan/images/technorati-small.gif" alt="" /> Technorati tags: <a href="http://technorati.com/tag/quicksilver" rel="tag">quicksilver</a> | <a href="http://technorati.com/tag/bluetoooth" rel="tag">bluetooth</a> | <a href="http://technorati.com/tag/applescript" rel="tag">applescript</a> | <a href="http://technorati.com/tag/automator" rel="tag">automator</a>)
    </p>

 [1]: http://robbevan.com/blog/2005/04/27/lifeblog/
 [2]: http://quicksilver.blacktree.com/
 [3]: http://www.frameworklabs.de/bluepush.html
 [4]: http://www.apple.com/macosx/features/automator/
 [5]: http://robbevan.com/blog/wp-content/uploads/Push2Phone.zip
 [6]: http://www.google.com/glm/gmail
