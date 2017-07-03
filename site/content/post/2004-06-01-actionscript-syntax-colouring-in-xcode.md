---
title: ActionScript syntax colouring in Xcode
date: "2004-06-01T07:22:24Z"
author: Rob Bevan
permalink: /2004/06/01/actionscript-syntax-colouring-in-xcode/
categories:
  - Software
---
(<span style="color: red;">New:</span> see also [ActionScript for TextMate][1])

I had this working previously in Project Builder, but the specification files were broken in [Xcode][2]. Thanks to the C# versions I found [here][3], I&#8217;ve been able to update these for Xcode. [This installer][4] adds two files, `ActionScript.pbfilespec` and `ActionScript.pblangspec` to `/Library/Application Support/Apple/Developer Tools/Specifications`, adding ActionScript syntax colouring and code completion (press opt-esc) to Xcode.

<div class="update">
  Update: <a href="http://blog.pixelconsumption.com">Sam Robbins</a> updated ActionScript.pblangspec to include component methods and properties. The installer now installs this updated version.
</div>

Personally, I now prefer to use [SubEthaEdit][5] as an external Xcode editor for ActionScript, as SubEthaEdit&#8217;s in-build ActionScript mode adds functions as well as classes to its symbols popup (Xcode can only see classes).

<div class="update">
  Update: and if, as I do, you find the colours in SubEthaEdit&#8217;s built-in ActionScript mode a little too garish (who wants bright red { operators }?), here&#8217;s <a href="http://robbevan.com/blog/wp-content/uploads/actionscript.mode.zip">a replacement</a>.
</div>

<del>Just copy the unzipped ActionScript.mode file to SubEthaEdit&#8217;s internal Modes folder, either manually by control-clicking SubEthaEdit and choosing &#8216;Show Package Contents&#8217;, then copying the file to <code>Contents/Resources/Modes</code> (you might want to back up the old ActionScript.mode first) or with this script (assuming you unzipped the file to your desktop): <code>mv ~/Desktop/ActionScript.mode /Applications/SubEthaEdit.app/Contents/Resources/Modes/ActionScript.mode</code></del>

<div class="correction">
  Correction: unless you want to replace the built-in version, copy the new ActionScript.mode file to one of:<br /> <code>&lt;br />
~/Library/Application Support/SubEthaEdit/Modes/&lt;br />
/Library/Application Support/SubEthaEdit/Modes/&lt;br />
/Network/Library/Application Support/SubEthaEdit/Modes/&lt;br />
</code>
</div>

 [1]: http://robbevan.com/blog/2004/10/09/actionscript-for-textmate/
 [2]: http://www.apple.com/xcode
 [3]: http://www.druware.com/products/xcodetools.html
 [4]: http://robbevan.com/blog/wp-content/uploads/asforxcode.pkg.zip
 [5]: http://www.codingmonkeys.de/subethaedit/
