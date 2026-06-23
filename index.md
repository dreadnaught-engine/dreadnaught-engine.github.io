---
layout: default
title: "Dreadnaught Engine Devlog"
---

# The Dreadnaught Architecture Ledger

This is the engineering journal for a high-performance, custom AAA-tier game engine written in C++23.

---

### Engineering Logs

<ul>
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date: "%B %d, %Y" }}</span> — 
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
