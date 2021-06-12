---
layout: layouts/post.njk
title: The History of the Dash Engine

date: 2014-04-29
published: false
tags: [prodstud, Dash]
---

**Note**: I wrote this in third-person to encourage future edits by other people. This article is copied on the [Dash wiki](https://github.com/Circular-Studios/Dash/wiki/Engine-History), which will remain up-to-date as time progresses.

### Graphos v1.0

![Graphos logo](https://github.com/ColdenCullen/dsa-pinball/raw/master/Graphos/Logo/Logo.png)

#### Time Period: Fall 2012
#### Team members: [Colden Cullen](https://github.com/ColdenCullen)

The first, rough version of the engine. An Intro to C++ class required Colden to create a game, so he went the extra mile to build an engine. It was used by [Danny Shumway](https://github.com/danshumway) to build a simple 2D game that was a cross between chess and checkers ("Cheskers", as it became known).

### [Graphos v2.0](https://github.com/ColdenCullen/graphos-v2)

#### Time Period: Spring 2013
#### Team members: [Colden Cullen](https://github.com/ColdenCullen), [Daniel Jost](https://github.com/PxlBuzzard)

This rewrite of Graphos brought a bevy of new features, such as a usable UI, dynamic object loading, and a (pseudo) maintainable architecture. Graphos began to have a distinction between game code and engine code, as well as having a folder structure outside the engine for game developers to utilize.

Colden brought Daniel Jost onto the project, who developed a painfully simple (and broken) pinball game using the engine. As it turns out, writing your own 3D physics system is a large undertaking.

### [Project 192 (Graphos v3.0)](https://github.com/ColdenCullen/Project-192)

#### Time Period: Fall 2013
#### Team members: [Colden Cullen](https://github.com/ColdenCullen), [Daniel Jost](https://github.com/PxlBuzzard), [Brandon Littell](https://github.com/BrandonLittell), [Eric Christenson](https://github.com/ericchristenson)

The third version had the four of us double-counting the engine for two classes, Game Graphics Programming and Data Structures and Algorithms 2. We saw the opportunity to really give engine development a shot, and (naively) make a cool game as well. We continued with the modular structure, and using proper version control methods kept everyone productive.

Project 192 is now infamous for us making a game from scratch to use for our final submission in about 10 manhours. It stands as a great testament to the power of the engine and the ability to use scripts to quickly create gameplay.

However, not all was well. The engine was becoming bloated with combined DirectX / OpenGL support and [V8](https://code.google.com/p/v8/) for scripting. C++ was giving us headaches. Daniel wanted to return to making games using the engine we built, and from our discussions about the future Dash was born.

### [Dash](https://github.com/Circular-Studios/Dash)

![Dash logo](https://cloud.githubusercontent.com/assets/512416/2726786/6618d624-c5c2-11e3-9049-23637e5a1739.png)

#### Time Period: December 2013 - Present
#### Team members: [Colden Cullen](https://github.com/ColdenCullen), [Brandon Littell](https://github.com/BrandonLittell), [Eric Christenson](https://github.com/ericchristenson), [Tyler Wozniak](https://github.com/zeDoctor), [Sean Brennan](https://github.com/ScrappyOrc), [Timothy Reynolds](https://github.com/tmr9209)

As the Project 192 team approached the end of the Fall 2013 semester there were mixed feelings about the engine. On the one hand we were happy with our accomplishments, but there were serious concerns around maintainability and scalability.

Colden and Eric drew the [D language](http://dlang.org/) out of a hat for a CS course during the fall. They began falling in love, and they were excited to sell Brandon and I on using it to do a full rewrite using D. A rewrite would also rid the engine of the bloat that had been building up over the last year and give a renewed focus on what the engine could be.

But what should Dash be? At first we thought it should be a résumé piece, but that seemed too short-sighted. Some sort of undergraduate capstone project to show the administration they should provide a more legitimate offering for large projects? Yes, but that's no way to focus an engine. A way to show game developers that C++ has competition? Definitely! What about giving back to the open-source community? Absolutely, the sharing of knowledge is the only reason any of us got to where we are now. And what have XNA/Monogame been up to since we started working on this? We could push the programmer-facing game engine aspect forward by providing modern features that can fill the gap between Monogame and Unity. Now we're talking.

With the vision for the engine, we wanted a game team to help drive early development and ensure Dash was easy to use for making games. Daniel asked around and pulled together a team of eight, all adept at the skills needed to make a 3D game. The Spectral Robot Task Force team and Dash teams formed Circular Studios to publish both projects.
