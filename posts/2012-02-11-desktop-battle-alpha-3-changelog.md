---
layout: layouts/post.njk
title: Desktop Battle Alpha 3 Changelog
date: 2012-02-11
tags:
  - Desktop Battle
  - games
---

![Desktop Battle Logo](http://res.cloudinary.com/danieljost/image/upload/v1381813108/desktopbattle_rp5914.png)

[DOWNLOAD DESKTOP BATTLE ALPHA 3](http://pxlproductions.com/desktopbattle/Alpha3.zip)

**How to make the game run:**

Open the .zip file, then drag/drop the “Desktop Battle” folder anywhere you want. Once it’s unzipped, open the folder and run “Desktop Battle.exe”.

**Controls:**

* WASD or Arrow Keys to move
* Move mouse and click to shoot
* Q to switch weapons

**Added:**

* Save and SaveData classes, used to Save/Load the game using serialized XML
  * The save file is in the game's install location, named savegame.xml
* Crosshair cursor
* Custom List, Stack, and Queue data structures
* Stack of bullets to recycle the same bullets in memory
* Queue of enemies that spawn into the room on an interval
* Remove all bullets onscreen when a new room loads
* Hero and Gun rotate to face the mouse
* New enemy: Key
  * Chases the Hero, has low hp

**Changed:**

* Moved the onscreen Bullet list and Bullet stack to Hero.cs
* Fixed ToString in Weapon and Sprite so that the names of the objects are properly displayed
* Made Room code able to handle multiple levels
* Enemies spawn farther to the right side of the screen
* The M16 now shoots bullets at an angle
* Improved weapon switching code to prevent crash early in the game
* Made the instructions in the first room easier to comprehend
