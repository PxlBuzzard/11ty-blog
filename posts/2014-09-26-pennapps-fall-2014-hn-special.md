---
layout: layouts/post.njk
title: PennApps Fall 2014 - HN Special

date: 2014-09-26
published: false
tags: [hackathon]
---

![PennApps X logo](http://res.cloudinary.com/danieljost/image/upload/v1411163941/pennapps_onrs3y.png)

Midnight. As I climb in bed to get a shortened night's sleep, my phone vibrates. A message from Dhruv Baid, Director of Travel & Outreach for PennApps, telling me that I have "more than 3 seats" to fill with last minute attendees. I reach out to my household (Danny, Tim, Sean, Rashele) with no takers, but through Sean's microphone in Destiny I manage to convince Colden. Colden suggests I ping Carl, who also accepts. Content with the amount of effort put forth at this late hour I go to sleep, only to be awoken at 5 am to go get on a bus.

On the bus, the three of us brainstorm ideas to hack on. My original plan before Carl and Colden signed on had been to add Firefox support to [HN Special](https://github.com/gabrielecirulli/hn-special), but that was meant to be a solo project. After awhile we come up with a couple good candidates: A Kinect joystick, where the player's body acts as an analog stick and their hands are buttons, and Guitar Hero + Kinect, which involves lining up 5 people and having them alternate between crouching and standing to play a note on the fret board.

One opening ceremony later, we speed-walk over to the hardware room and grab two Kinects. We rip into the Kinect SDK and quickly get a demo program running that overlays a skeleton onto each person in the scene. Success! Or... wait? Why did it crash there? Try putting your hand on top of me again. Yep, that did it!

It turns out even with the new Kinect, the software cannot handle more than 3 people without crashing. No more Guitar Hero modification. But what about the human joystick? A little bit of searching led to find [it exists](http://projects.ict.usc.edu/mxr/faast/) already.

![Sleep deprivation effects us all.](http://res.cloudinary.com/danieljost/image/upload/v1411006045/10672317_10152709978534120_4941469359236816693_n_n0nyzm.jpg)

Carl, Colden, and I went for a midnight stroll to discuss our options. We had only burned four hours of hacking, but without another project that we were passionate about building, things felt grim. What if we got started with tools for [Dash](https://github.com/Circular-Studios/Dash)? No, we should save that for later. Revisit [Stats At Last](https://github.com/PxlBuzzard/StatsAtLast) (my last PennApps project)? Nah, the others don't have the same passion I do about seeing that come to fruition. Something with a drone? Oculus Rift? Leap Motion? But all the quick projects you can build for that hardware have been done already!

Eventually Colden agrees to hack on [HN Special](https://github.com/PxlBuzzard/hn-special) with me. Carl decides to use the time to start learning [Swift](https://developer.apple.com/swift/), Apple's latest programming language, to build a food and wine pairing app for iOS.

Meager amounts of sleep and a couple massages later (they had massages on Saturday!), we arrive at the expo floor Sunday morning to show off our efforts.

![Expo floor. You can see me in a purple shirt on the center right. Original: https://secure.flickr.com/photos/mager/15052189150/in/set-72157647524545851](http://res.cloudinary.com/danieljost/image/upload/c_scale,w_900/v1411009883/15052189150_097fbb5223_o_or90pr.jpg)

Colden and I show off our work to a grand total of 4 people: a judge, a college freshman, a Mozilla rep, and [Nick from SendGrid](http://sendgrid.com/blog/author/nicholas/) (better known as "the happiest person on the planet"). Plenty of passersby looked into the screen, marveling at the pixels within. After a little bit we packed up and meandered around. I quickly noticed a pattern: I only stopped to look at "fun" projects. Inevitably all those projects involved a hardware component. The most stark moment came as I waited to try out a [Myo](https://www.thalmic.com/en/myo/) hacked to work as a mouse, and a PennApps Health Hack at the next table had zero visitors.

Hardware, especially bleeding-edge technology, has an inherent draw to it. That's likely why we wanted to hack on a Kinect v2, and why many of the top 10 finalists utilized new hardware. Yet only one of the top 10 hacks actually had a health care application: [Scolio](http://challengepost.com/software/scolio). Most of the flashiest hacks aren't going to be useful outside of a hackathon demo. Heck, even our Kinect projects were concieved as projects that would be fun demos rather than actually being useful to anyone.

This approach to hackathons feels wrong, or at least like we're missing the mark. Ben Cohen, a fellow RIT hacker and PennApps attendee, phrased the issue as "hackers building tools for hackers." We stay in our bubbles, and initiatives like PennApps Health Hacks can only convince so many people to leave the bubble. What we need is a hackathon that champions projects intended to benefit the larger non-hackathon community. [Random Hacks of Kindness](http://www.rhok.org/) and [Software Freedom Day](http://www.softwarefreedomday.org/) are two examples of events geared towards this mindset, but the largest school-sponsored hackathons are the ones that stand the most to gain from reorienting their goals. I am hopeful that [Brick Hack](http://brickhack.io/), RIT's first school-wide hackathon, will share this mindset of promoting projects that do good for the world, not just one-off hacks for a show floor demo.
