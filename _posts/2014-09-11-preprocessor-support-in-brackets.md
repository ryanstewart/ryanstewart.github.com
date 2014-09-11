---
layout: post
title:  "Preprocessor Support in Brackets"
date:   2014-09-11 1:00:00
categories: brackets adobe preprocessors
---
I've loved Brackets from day 1, but as someone who uses Sass for nearly all of his personal projects, the lack of preprocessor support has ranged from a minor inconvenience to a real pain. And that's one of the reasons I'm incredibly excited about the latest release of Brackets. We've started to add support for preprocessors to some of Brackets' innovative features. 

The latest release (Release 43) adds support for LESS and SCSS files when you're using Quick Edit, Jump to Definition, and Live Highlight. The one I'm most excited about is Quick Edit. Now when you're using the inline editors to see the code that applies to a particular element or class, you'll see your LESS or SCSS files alongside the processed CSS files. That means you can jump directly to your preprocessor code where the styles are actually defined, edit those, recompile them, and see the changes. 

I'm also stoked about the live highlight feature for LESS and SCSS. With it you can put your cursor on a definition in your LESS/SCSS files and if you're in live preview mode you'll see the live highlight box in all the places that definition applies. It's a really nice way to see where your preprocessor styles are actually being applied.

I did a quick video (below) showing some of these in action. We've got a lot more planned. I want to get regular Sass syntax support for these features as well as see if we can make Live Preview work with preprocessors. 

<iframe width="640" height="480" src="//www.youtube.com/embed/cEiORP1uG5I" frameborder="0" allowfullscreen class="center"></iframe>

=Ryan