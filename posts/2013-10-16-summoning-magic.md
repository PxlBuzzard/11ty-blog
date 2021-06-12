---
layout: layouts/post.njk
title: Summoning MAGIC

date: 2013-10-16
published: false
tags: [MAGIC, Web Development]
---

> "Dark, mysterious, and magical." - Andy Phelps

## In the beginning

I left my first meeting with [Andy](http://magic.rit.edu/users/andy/), the Director of the MAGIC Center at RIT, with those words ringing around in my head. I was trying to decipher exactly what that meant in terms of web design, much easier said than done. After a couple days, my personal whiteboard showcases my lamentable attempt at cracking the code:

[![Initial whiteboard thoughts on MAGIC](http://res.cloudinary.com/danieljost/image/upload/v1381977563/whiteboard_magic_a4focx.jpg)](http://res.cloudinary.com/danieljost/image/upload/v1381977563/whiteboard_magic_a4focx.jpg)
*Yes, easter eggs were on my mind really early on.*

Looking back I see that a lot of of those early ideas were actually exactly what I needed, but at the time it felt like I was bumbling around in the dark. My saving grace throughout the process was working with [Elouise Oyzon](http://weez.oyzon.com/), or Weez. At the beginning she freed me from the task of coming up with the front-end conceptualization and let me focus on doing something I have never done before: the back-end of web development. Because I was the only developer on the project (Weez did design and Andy was our grader), I had no one to verify my sanity as I made decisions about how the site would be built. And so, like any good upstart will do, I researched.

[![List of bookmarks for MAGIC](http://res.cloudinary.com/danieljost/image/upload/v1381977465/bookmarks_r6qcjl.png)](http://res.cloudinary.com/danieljost/image/upload/v1381977465/bookmarks_r6qcjl.png)
*Most of these links were amassed within the first week of work when I was just bookmarking anything that was a [website-name].io link. When did .io catch on so much?*

## Design

The first page Weez concepted was our project page, since we thought that would be a page of critical important and be relatively easy to figure out the final requirements early on. It turns out we weren't that far off from the final release, as you can see below. In fact, every page turned out very close to the original concept other than the homepage, which saw more than its fair share of designs leading right up to launch.

[![Weez's project concept](http://res.cloudinary.com/danieljost/image/upload/v1381979477/project_concept_uivfji.png)](http://res.cloudinary.com/danieljost/image/upload/v1381979477/project_concept_uivfji.png)

[![The final page](http://res.cloudinary.com/danieljost/image/upload/v1381979480/project_final_fwvhvh.png)](http://res.cloudinary.com/danieljost/image/upload/v1381979480/project_final_fwvhvh.png)

## The tech stack

I spent a good amount of time digging around in front-end land ([Supersets](http://sass-lang.com/) [of](http://lesscss.org/) [CSS](http://learnboost.github.io/stylus/) are amazing). I googled around for a lightweight content management system to find the latest and greatest. I've previously used [Wordpress](http://wordpress.org/) and [Concrete5](http://www.concrete5.org/), but while they both served their purpose well MAGIC required a feature-set more tailored towards data management and dynamic page generation. I bumped into [Django](https://www.djangoproject.com/) early on, but without understanding what it offered (the automatic admin interface was the main reason I bookmarked it) I moved on and scoped out my options. Eventually I found [Django CMS](https://www.django-cms.org/) and was hooked. Super-easy page building and plugin editing fulfilled the requirement of making the site easy to expand and grow for years to come without needing a dedicated web team to add new content.

The server is using Red Hat Enterprise Linux with Apache, MySQL, and Python (RAMPy). Django powers the website that is built using [Foundation](http://foundation.zurb.com/) and SCSS. It was a worthwhile adventure learning how to set up a linux box from scratch, even with hiccups like getting mod_wsgi and SASS to work properly (no documentation and needed to write a special bash script, respectively).

## Going forward

The site started as a summer co-op. Andy kindly offered me part-time hours for the fall semester, and a good thing he did since the site launched a month later than we anticipated. As I finish out the semester there are tasks both large and small, such as adding support for project pages to embed games via Unity or Flash player.

On a personal level, this project revitalized my passion for web development. I had all but sworn off working on websites in order to focus myself on gameplay programming, but after MAGIC I have learned that there is so much more underlying technology to tinker with and the industry is just as passionate about their work. Innovation is key for both the web and games, and I want to play a part in that. And, coincidentally, the opportunity to innovate is exactly what Andy and MAGIC are giving to students.
