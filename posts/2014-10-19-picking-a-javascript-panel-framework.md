---
layout: layouts/post.njk
title: Picking a JavaScript Panel Framework
date: 2014-10-19
tags:
  - web development
  - javascript
---

> This post was originally sent as a response to [Jeff Houde](https://github.com/Lochemage), the developer of wcDocker, who asked why I didn't pick his framework.

Initially when I set out to find a framework to create web-based game development tools, I found [DockSpawn](http://www.dockspawn.com/) and [wcDocker](https://github.com/WebCabin/wcDocker). DockSpawn had a better first impression, which I will credit to a fairly pretty website that has code examples and documentation, as well as the framework being easier on the eyes. I also like the panel docking that closely resembles Visual Studio.

I ultimately made the decision to use wcDocker over DockSpawn because you were still actively developing (the last update to DockSpawn was in February 2014) and because I have more experience with Javascript over Dart. Also I wanted to experiment using [Bower](http://bower.io/) for developing a project, and integrating that into wcDocker so that I could see how Bower works from both the perspective of a package developer and a package consumer sounded like a perfect setup.

And it was a perfect setup! I got to see and [fiddle with the internals](https://github.com/WebCabin/wcDocker/pull/11) of wcDocker, and help clean it up where I could. Figuring out how to "modify" another script ([jQuery-contextMenu](http://medialize.github.io/jQuery-contextMenu/)) without actually touching the source was a great lesson, albeit it one that I had to rely on my friend [Danny Shumway](https://github.com/danShumway) to help solve. So good times, let's build with wcDocker using Bower.

Then [Golden Layout](https://golden-layout.com/) appeared on [Hacker News](https://news.ycombinator.com/item?id=3D8400265). I hadn't done anything more than combining wcDocker and [React](http://facebook.github.io/react/) on my [own project](https://github.com/Circular-Studios/dash.js), so I was still at a point where I could switch frameworks. Both frameworks are trying to solve the same problem, but Golden Layout had examples, tutorials, documentation on top of being in active development, looking as pretty as DockSpawn, and having (somewhat) cleaner code structure for developers. [I was concerned](https://news.ycombinator.com/item?id=3D8402663) that the project wasn't hosted anywhere but his own website, but he began hosting [on Github](https://github.com/hoxton-one/golden-layout) shortly thereafter. I am still concerned that he is using a Creative Commons license on his code, as that is unexplored legal grounds. Concern aside, I chose what I thought was the best framework available at the time.
