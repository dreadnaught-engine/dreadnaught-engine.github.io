---
layout: default
title: "Home"
---

<style>
  /* Changelog Table Styles */
  .changelog-table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 20px;
    font-family: monospace;
    font-size: 0.9rem;
  }
  .changelog-table th {
    text-align: left;
    color: #8ab4f8;
    border-bottom: 2px solid #14203d;
    padding: 10px;
  }
  .changelog-table td {
    padding: 10px;
    border-bottom: 1px solid #14203d;
    color: #c4d4e6;
  }
  .version-tag {
    background-color: #0d152b;
    color: #00ff66;
    padding: 2px 6px;
    border: 1px solid #00ff66;
    font-weight: bold;
  }
  .view-all {
    display: block;
    margin-top: 15px;
    color: #d600ff;
    text-decoration: none;
    font-family: 'Rajdhani', sans-serif;
    font-weight: bold;
    text-transform: uppercase;
  }
  .view-all:hover { text-decoration: underline; }
</style>

# Welcome to the Dreadnaught Engine
This is the engineering journal for a high-performance, custom AAA-tier game engine written in C++23.

## Recent Engineering Milestones
<table class="changelog-table">
  <thead>
    <tr>
      <th>Version</th>
      <th>Date</th>
      <th>Update</th>
    </tr>
  </thead>
  <tbody>
    {% assign releases = site.posts | where: "status", "release" | limit: 5 %}
    {% for post in releases %}
    <tr>
      <td><span class="version-tag">{{ post.version }}</span></td>
      <td>{{ post.date | date: "%Y-%m-%d" }}</td>
      <td><a href="{{ post.url }}" style="color: #c4d4e6;">{{ post.title }}</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>
<a href="/devlog" class="view-all">>> View Full Changelog</a>

---

## Site updates

2026/06/24 - Updated homepage, added footer. <br>
2026/06/23 - Created the site and added placeholder pages.

---

Hello and welcome to the development page for the Dreadnaught Game Engine! You can call me JACK, and I'm learning how to code through the development of this engine. I'm using this blog to help with the production of my project. 

As of 06/24/2026 I am still in the design phases of the engine. I have a general idea of what I want my game to eventually be, but I want to work out the systems before I commit to any code. I'll be updating the site intermittently mostly for personal reasons, but I'm making it public just in case anyone is curious about this project.

First and foremost: *why?* Why not use Unreal, Unity, or even Lumberyard? tl;dr I'm picking this up as a hobby. Every kid who played video games at an early age always dreamed of creating their own game, and for me, that dream has never passed. I would think that playing video games would be sommething I would no longer do as I got older, but I still enjoy what game devs have to offer. Video games have become a passion, something I could talk about for the rest of my life, but I never had the time or motivation to pursue the creation of one. Just thinking about 3d modeling gives me a headache. You're telling me I have to learn this skill for 2 years before I can model this floppy cock on a mimic chest? No thanks.

But then AI had recently been making waves of progress. At first it was pretty garbage - telling people to go seppuku themselves - but now it has gotten pretty advanced. Yes, I'm vibecoding, but why would I waste my time trying to hammer a nail with my hands when I can hire someone to do it for me? I'll be testing the limits of how far I can go, and eventually learn how to code myself, or at the very least understand the logic and structure of everything.

I want to make myself clear: this is a personal project. I fully intend to release my game(s) for free with purchasable cosmetics, but I'm going in assuming nobody will even pick up my game. I am making a game *I* want to play. If others want to play it too, great! If not, that's fine! If I started a woodworking hobby and made a furniture set, why would I be upset if nobody used it? I built the set for *me*. 

Anyway, if you're confused about the two changelogs, the top one links directly to the Devlog and the other one is just minor quick text edits I type out myself. 

Maybe I'll finish this project some day, maybe not. Better to die trying than regret not even making an attempt for the rest of my life.

Signing out,<br>
JACK
