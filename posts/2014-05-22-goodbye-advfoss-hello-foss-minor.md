---
layout: layouts/post.njk
title: Goodbye Advfoss, Hello FOSS Minor

date: 2014-05-22
published: false
tags: [advfoss]
---

**tl;dr** Advanced FOSS went so well I'm going to cram a minor into my last semester this fall.

But let's back up. Even as a younger kid I was enraptured with the game modding community, which is effectively the most open-source success the game industry has seen so far (I'm rooting for the new Unreal Tournament and Cards Against Humanity doesn't count). Last summer I had the privilege to develop the website for the [MAGIC Center](http://magic.rit.edu/main/index.html) on my own. I had a list of requirements, and the Internet was my oyster as far as technology goes. The full story deserves a blog post for another day, but the biggest takeaway was that open-source development is primetime.

When I approached Remy about skipping the pre-req to jump straight into Advfoss he was happy to agree. Colden and I had been working with him to bring [qlt](http://qlt.rit.edu) to RIT (it's an open-source Learning Management System). The class was an opportunity to expand my open-source knowledge and contribute to the greater Internet, and that's just what I did. Bringing [Oculus-D-Rift](https://github.com/Circular-Studios/Oculus-D-Rift) and [D language for Atom](https://github.com/ColdenCullen/atom-dlang) to the world would not have happened without this class. I also open-sourced [my own website](https://github.com/PxlBuzzard/danieljost.com) and made a PennApps project, [StatsAtLast](https://github.com/PxlBuzzard/StatsAtLast), open-source from the outset. Heck, I even solved a problem I had by writing [nunjucks-brunch](https://github.com/PxlBuzzard/nunjucks-brunch) over a weekend.

![Dlang for Atom](https://res.cloudinary.com/danieljost/image/upload/v1400785135/Screen-Shot-2014-05-22-at-2-57-14-PM_t3aivm.png)

*Dlang for Atom*

I have plenty more to share about why Free and Open Source Software is awesome, and I'm sure next semester as I'm doing three FOSS classes to become one of the first people in the country to graduate with this minor I will write all about it.

## Issues closed from my [last post](http://blog.danieljost.com/final-countdown-to-advfoss/):

### [PuzzleDash](https://github.com/zeDoctor/PuzzleDash) - [Add installation instructions to README](https://github.com/zeDoctor/PuzzleDash/issues/1)

It turns out this was a waaay more useful commit than I intended. Once we went live PuzzleDash was the main game we had to show off what a "regular" game repo looks like for a Dash game.

### [danieljost.com](https://github.com/PxlBuzzard/danieljost.com) - [Update and improve homepage](https://github.com/PxlBuzzard/danieljost.com/issues/5) - [Update projects page](https://github.com/PxlBuzzard/danieljost.com/issues/4) - [Add a README](https://github.com/PxlBuzzard/danieljost.com/issues/3)


### Extra: Added [Travis](https://travis-ci.org/PxlBuzzard/danieljost.com)

My website was about a semester out-of-date and needing some freshening. Adding Travis and switching my webhost to [Amazon S3](http://aws.amazon.com/s3/) has resulted in fast, up-to-date, auto-compiling website. I have plans to lessen the dependencies (i.e. move off of Jekyll) as my next big step forward, as well as a front-end redesign.

### [Sample Dash Game](https://github.com/Circular-Studios/Sample-Dash-Game) - [Add a camera script](https://github.com/Circular-Studios/Sample-Dash-Game/issues/3)

This is still in its own branch and therefore not a closed issue, but it will bring a legitimate camera to Dash's sample game, helpful for both debugging the engine and showing the power of scripts.
