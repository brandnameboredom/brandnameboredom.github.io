---
layout: post
title:  "Customizing Eclipse"
date:   2016-06-29 12:00:00 -0400
categories: [Eclipse, Customizations]
author: Brad Turner
---

One of the most frustrating things for me when transitioning from the default setup in [Visual Studio] to [Eclipse] has been the change in keybindings for toggling a breakpoint.  I tried setting the "Toggle Breakpoint" key binding in 

> _Window_ -> _Preferences_ -> _General_ -> _Keys_ 

but it did nothing for me while my cursor was active in the editing window.  A quick Google search and I stumbled upon [this](http://stackoverflow.com/a/3605724/70130) answer on [StackOverflow].  Turns out, key bindings are related to the perspectives in Eclipse and I needed to enable the "Breakpoints" command group for my perspective.  So, 

> _Window_ -> _Customize perspective_ -> _Command Groups Availability_ 

and select "breakpoints".  Now, my custom binding of F9 to the "Toggle Breakpoint" action is usable from the editor window.  Sweet.

[Visual Studio]: https://www.visualstudio.com/
[Eclipse]: https://eclipse.org/
[StackOverflow]: http://www.stackoverflow.com