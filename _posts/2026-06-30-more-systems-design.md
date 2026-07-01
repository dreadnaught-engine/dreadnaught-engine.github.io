---
layout: post
title: "Devlog #2 - More Systems Design!"
author: "JACK"
status: release
date: 2026-06-30
version: 0.0.0
tags: [Player, Systems, Multiplayer]
---
# The design must flow

These past few days have been nothing but game design. Yesterday I finished 4 designs that are player-centric, and I think 4-5 days ago I got an idea of how parkour and movement in general worked. Today I refined a bunch of my systems but most of the time I've been battling with the design because I want multiplayer enabled in the game.

But because I want multiplayer, the entire structure of the engine suddenly flipped. Now, everything must be server-authorized with 0 client-trust. Single player mode should be fine, but multiplayer enabled modes open the door to an entirely different dynamic. One example is hard-coded faction cities - only online-enabled players get to go there. I might consider enabling them for a completely single player hosted mode, but I want the multiplayer done first because the restrictions and architecture must comply with network streams.

<figure style="text-align: center;">
  <img src="{{ '/assets/images/todd.jpg' | relative_url }}" alt="Description of image" style="max-width: 100%; height: auto;">        
  <figcaption>"FUCK YOU" -Todd Howard of Bethesda Games</figcaption>
</figure>   

On a personal level, I'll be starting classes again tomorrow, so working on this engine will come to a massive slow-down, but this is a marathon not a race. Hobbies are a personal endeavor, and rushing things will just cause burnout. 

Speaking of, there's a Burnout mechanic I've devised for NPC workers at a player base. If you've played games like Rimworld, you basically assign priorities to a Pawn (NPC) and they choose actions based off of priorities. The issue is, if you have one person with a high priority, they will only commit to that job, even if they like other things or are skilled at other things.

So I decided that pawns can switch their jobs every once in a while with a "Burnout" mechanic. Mathematically it's very simple, so it shouldn't take up that much performance, and I hope to see an NPC of mine one day taking a much needed vacation on their own! This isn't real life, they're not bound to the cubicle, they can act as they wish. 

-JACK
