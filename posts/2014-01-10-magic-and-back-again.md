---
layout: layouts/post.njk
title: MAGIC and Back Again
date: 2014-01-10
tags:
  - MAGIC
  - web development
  - advfoss
---

I set out to pick the best framework for the RIT MAGIC Center. After finding [Django CMS](https://www.django-cms.org/en/), I thought I had found my answer in [Django](https://www.djangoproject.com/). Easy content management, an automatic admin interface, easy database models, a forward-thinking HTML templating system, and a generous open-source community all contributed to my decision, but ultimately I made some choices that didn't work out in the end.

#### What went wrong?

Django is stable. Backwards-compatible. Well-documented. Widely-used.

The plugins are a different story.

The Django community is full of motivated developers doing a great job of writing applications that run on the platform. I had the pleasure of talking to many developers and contributing code fixes upstream. I mean no ill-will towards those people who put their time and energy into making the world a better place through open-source software (OSS).

The issue when working on a site like MAGIC is that there are a lot of moving parts. Different plugins all come with different dependencies, from the version of Python required (we use 2.6), to a simple datetime app that two apps need two different versions of. A small, focused site should be able to handle small fixes, but for something as complex as MAGIC is (and wants to become), a significant portion of time ends up spent fixing bugs instead of developing new features.

Documentation is the other problem of open-source at large. Efforts like [Read the Docs](https://readthedocs.org/) go a long way towards simplifing the process for developers. However, many developers often assume their codebase is their documentation. While that can and should be true, it is critical to maintain pages explaining your design philosophy, a roadmap, and other non-code concerns.

## Why switch off of Django?

The MAGIC Center needs a web presence. When you have a large codebase that has little bugs and workarounds scattered throughout the stack, you have a bad stack. MAGIC has since converted the website to be static HTML, a decision rooted in the knowledge that it is difficult for a static website to break randomly (at least the webcode part). It isn't as fast or easy to update as a solid CMS like Wordpress or Drupal ("fast" and "easy"), but it works in the meantime. Uptime and load times are paramount to any website, and my implementation of Django failed on both counts. I still believe that with the right setup Django would provide a solid foundation for MAGIC.

## What did you learn?

What a great question to ask at this point in the post.
