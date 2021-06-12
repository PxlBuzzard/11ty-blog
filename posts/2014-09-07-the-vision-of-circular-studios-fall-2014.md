---
layout: layouts/post.njk
title: The Vision of Circular Studios, Fall 2014

date: 2014-09-07
published: false
tags: [Dash, Spectral Robot Task Force, Circular Studios]
---

For those of you who don't know me: I'm Daniel Jost, a fourth year Game Design and Development student at the Rochester Institute of Technology. I am the Producer of Dash and Spectral Robot Task Force, as well as the Lead Programmer for Spectral. Both are products of Circular Studios.

## What is Circular Studios?

At its core, [Circular Studios](http://circularstudios.com/) is a group of past and present RIT students who want to make cool stuff, namely games and game technology. Given the nature of school we have alumni working at places such as [Microsoft](http://microsoft.com), [Logitech](http://www.logitech.com), and [High5Games](http://www.high5games.com/). This semester (Fall 2014) we have 6 students working on Dash and 6 on Spectral, as well as a couple administrative folks helping with marketing and other tasks.

## What is Dash?

![Dash logo](http://res.cloudinary.com/danieljost/image/upload/v1410025161/dash-logo_uhbumk.png)

[Dash](https://github.com/Circular-Studios/Dash) is a free and open source 3D game engine. I've previously written a [history](https://github.com/Circular-Studios/Dash/wiki/Engine-History) of how Dash came to exist in the first place if you are interested. Rather than answer what Dash is, I want to talk about what Dash will strive to be after this semester:

* One of the first open source implementations of [Physically Based Rendering](http://www.marmoset.co/toolbag/learn/pbr-theory).
* The de facto (and first) 3D game engine written in the [D language](http://dlang.org/).
* A robust engine for game programmers and designers, by providing a simple game scripting system and visual tools for designers.
* A [WebSockets](https://en.wikipedia.org/wiki/WebSocket) API, allowing game developers to create custom tools in any language and framework they choose.

We entered this semester on version 0.9.0, which represents a lot of milestones full of features already shipped. Our goal is to reach **1.0.0** by the end of the semester, which we have defined as: **a game developer can use Dash to create a game without needing to contact our team**. This means we need great documentation and complete unit tests on top of all the features one would expect a game engine to have.

## What is Spectral Robot Task Force?

![Spectral banner](http://res.cloudinary.com/danieljost/image/upload/v1410025161/spectral_banner_naky8g.png)

Spectral Robot Task Force a turn-based strategy game. If you would like to see more about the story and some screenshots, the [Circular Studios website](http://circularstudios.com/) has your back.

The dawn of Spectral came from my desire to return to game development after spending a semester working on a game engine with no game to show for it. We all agreed that Dash would benefit from a team of developers using the engine during development to properly evaluate it for its intended purpose: game development. It keeps motivation high for an engine programmer to know that their feature will be used as soon as it is complete, and more importantly ensures that programmers aren't wasting their time working on code that will never be utilized.

![A gif I made after we had movement around tiles working.](http://i.imgur.com/cN8Qp0H.gif)

*The image above was made after I first got tile movement working circa April 2014.*

After a relatively successful spring semester, we completed a playable prototype of the game and demonstrated it at [Imagine RIT](http://www.rit.edu/imagine/planyourday14/exhibit.php?id=114).

#### So what's the plan this semester?

This is the first time any of us has had the opportunity to work on a game for longer than one semester (or quarter). I'm really excited to already have a codebase, design document, and a playable game going into a semester. Our designers now get a chance to iterate on the gameplay (for example, we are switching to a hex grid instead of squares). Art can continue to be made with the previously established pipeline. Code can be refined and supplemented with new features. Features included, but not limited to:

* Weapons
* Customizable stats and loadouts
* Singleplayer quests / scenarios
* Hotseat and asynchronous multiplayer
* Terrain elevation
* AI

Spectral should move beyond prototype into a game that people actually want to play. With improvements to Dash, combined with our awesome artists, it will include some of the best graphics seen from a student project. This will be the showpiece that proves Dash is ready to be used in production game development, and it will be the most complete game any of us have done in school.

## The Dream

Dash has already grown tremendously beyond what we thought possible when we started the project. In the last two weeks, which have been pretty inactive, the Github page has pulled in [2,256 views](https://github.com/Circular-Studios/Dash/graphs/traffic). That's crazy!

When we ship v1.0.0 I want the Internet to explode. The D language has been nipping at the heels of C++ for too long, and Dash + Spectral ought to provide a convincing argument for D being the next great language. I want Circular Studios to be contacted by Wired, get featured on Gamasutra, and be invited to speak at [DConf](http://dconf.org/). Dash and Spectral should be showcased in the RIT booth at the Game Developers Conference. Heck, while we're dreaming, I want to see a commercially successful game ship that uses Dash (that isn't Spectral).

Speaking of RIT, the professors in the IGM department took a chance on us. A big chance. Student projects larger than five people fail more often than not, and we had *14* people last semester. Through whatever success our team garners, I hope that IGM receives credit by attracting more talent, both incoming students and faculty. Professor Schwartz, thank you for everything you did for our group, directly and indirectly. I would not be writing this had you not been so influential.

Alright team, let's buckle in and get going.
