---
title: Comment using the Skype API
date: "2005-11-12T18:49:19Z"
author: Rob Bevan
permalink: /2005/11/12/comment-using-the-skype-api/
categories:
  - Software
---
I spent some time yesterday playing around with the [Skype API][1] because I wanted to see if I can initiate text-to-speech calls for [a project][2] we have in development.

Seems like the [Mac OS X API][3], like the [Skype][4] app itself, lags a little behind the Windows/Linux versions and the Applescript interface (which is easiest to use from a cgi script) is only partially implemented.

I did manage to get a simple web-based IM sending app running on OS X server. Try this form to Skype and I&#8217;ll post your message here as a comment:

<strike>This obviously only works if I&#8217;m online too.</strike> Seems to get queued in the Skype cloud even if I&#8217;m not.

(I&#8217;m not providing a generic web to Skype gateway here, for that try [InstantSkype][5].)

<div class="update">
  <p>
    Update: see my Skype <a href="http://forum.skype.com/viewtopic.php?t=29120&#038;start=0&#038;postdays=0&#038;postorder=asc&#038;highlight=">forum post</a> on why managing calls with the Applescript interface is a problem.
  </p>
</div>

 [1]: http://share.skype.com/share/developer_blog/
 [2]: http://www.xpt.com/uk/work/the-nuuk/
 [3]: http://share.skype.com/developer_zone/documentation/skype_api_for_osx/
 [4]: http://share.skype.com/in/102/171559
 [5]: http://skyperunners.com/instant/
