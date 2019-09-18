---
layout: post
title:  "Cloud 9"
date:   2019-08-20 12:00:00 -0400
categories: [AWS, Cloud9, IDE]
author: Brad Turner
---

I've never really had a desire to look into cloud based ide solutions.  I used more traditional IDEs (Visual Studio, Eclipse, etc.) in the past professionally and I've never really cared for the bloat.  I found myself focusing on the IDE (plugins, customizations, etc.) rather than the problem I was there to solve.  These days I'm primarily using the Jet Brains suite (Rider/Web Storm/Data Grip/etc.) professionally and VS Code for small things.  Recently, however, a friend of mine passed along a tutorial for deploying a modern web app architecture to AWS which suggested the use of Cloud9.  I have to admit, Cloud9 is pretty sweet.

- Cloud9 deploys to an EC2 instance
- "Session Timeouts" result in resource shutdown so you don't pay for stuff you aren't using
- AWS cli integration out of the box
- Docker integration out of the box
- relatively speedy (even on a free tier t2.micro instance)

I'm intrigued to see how the collaborative portion of Cloud9 works.

Now, to explore other cloud-based IDE options.  I'm looking at you che.