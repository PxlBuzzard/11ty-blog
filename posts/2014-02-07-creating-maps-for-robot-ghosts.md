---
layout: layouts/post.njk
title: Creating Maps for Robot Ghosts

date: 2014-02-07
published: false
tags: [Robot Ghosts]
---

The general features needed from any level editor are:

* Load levels (yaml files)
* Easily map to a 2D grid
* Custom object placement outside the grid system
* Tile types: spawnable, walkable, obstacle, etc
* Deal with incorrect / garbage / malicious data (mostly incorrect)

With that in mind, here are some suggestions for tools that we are mulling over:

#### [Tiled](http://www.mapeditor.org/)

Pros: Open-source, customizable, GUI
Cons: No 3D, needs multiple converter scripts to be written to work for our needs

#### [GtkRadiant](http://icculus.org/gtkradiant/)

Pros: Open-source, 3D, used for some popular games
Cons: Toolchain is probably way outside our scope

#### In-game level editor

There are some interesting things we can do if we roll our own editor. Foremost, we can ship the game with a built-in level editor. This would also allow for the fastest iteration of level design and testing.

Features specifically for an in-game editor:

* Save a level (as a yaml file)
* In-game editing of everything
* Model placement, and object types (obstacle, special, etc)
* Spawn, walk, obstacle tiles
* Map size, name
* A GUI to display this all nicely

Pros: Does exactly what we want it to do with no unneeded features
Cons: We have to make it

### What to choose?

We will be exploring all available options and coming to a decision in the next couple weeks. Everyone agrees that an in-game editor would be amazing, but it may well involve the most amount of work and time. Stay tuned!
