---
layout: layouts/post.njk
title: Post-mortem - qlt
date: 2014-06-17
tags: web development
---

qlt is a fork of [Canvas](https://github.com/instructure/canvas-lms), an open-source learning management system. If you've used Blackboard, D2L, MyCourses, that's what Canvas is.

Colden, Weez, and I were drawn to Canvas for a few reasons. For one, open-source software is awesome. Canvas is a great LMS on its own, and being open-source only sweetened the deal. Canvas was designed to be a user-first LMS, and that vision effects every nook and cranny. It's fast, simple for newcomers, and powerful for skilled users.

Instructure, the creators of Canvas, have a hosted offering with support and hosting for a fee. Sadly, their public documentation was lacking (whether or not it was due to focusing on the hosting side I can't say), especially when it came to anything deeper than the initial install. Even the initial install could have been greatly expedited with packages for various operating systems, but instead you are stuck installing the dependencies and creating the configurations yourself.

qlt chose to be a fork in order to make modifications to the codebase. Weez requested a custom view for students looking at a course (kind of a magazine view) as well as an easy way for students to connect to Google Hangouts for office hours. The custom view was almost finished, and the Google Hangouts plugin worked well considering we didn't have the official API docs available.

I would love if RIT considered switching away from MyCourses to Canvas. The open-source nature would allow enterprising hackers to make the system better, RIT wouldn't have to pay for an LMS, and the experience is just better day-to-day.
