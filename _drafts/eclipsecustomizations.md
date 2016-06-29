---
layout: post
title:  "Customizing Eclipse"
date:   2016-06-29 12:00:00 -0400
categories: [Eclipse, Customizations]
author: Brad Turner
---

One of the most frustrating things for me when transitioning from the default setup in [Visual Studio] to [Eclipse] has been the change in keybindings for toggling a breakpoint.  I know, it sounds minor but it proved to be a pretty significant pain point for me.  I tried setting the "Toggle Breakpoint" key binding in Window -> Preferences -> General -> Keys but it did nothing for me while my cursor was active in the editing window.  A quick Google search and I stumbled upon [this](http://stackoverflow.com/a/3605724/70130) answer on [StackOverflow](http://www.stackoverflow.com).  Turns out, key bindings are related to the perspectives in Eclipse and I needed to enable the "Breakpoints" command group for my perspective.  So, Window -> Customize perspective -> Command Groups Availability and select "breakpoints".  Now, my custom binding of F9 to the "Toggle Breakpoint" action is now usable from the editor window.