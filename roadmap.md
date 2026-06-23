---
layout: default
title: Roadmap
permalink: /roadmap
---

# Engine Development Roadmap

<p>Tracking the architecture and implementation of the Dreadnaught Engine.</p>

<div class="roadmap-container">
  {% for part in site.data.roadmap %}
    <h2 class="roadmap-part-title">{{ part.title }}</h2>
    
    {% for item in part.items %}
      <details class="roadmap-item status-{{ item.status }}">
        <summary>
          <span class="status-icon"></span>
          <span class="item-id">{{ item.id }}</span> 
          <span class="item-name">{{ item.name }}</span>
        </summary>
        <div class="item-content">
          <p>{{ item.desc }}</p>
          {% if item.link != "" %}
            <a href="{{ item.link }}" class="btn-read-more">>> Read Engineering Log</a>
          {% endif %}
        </div>
      </details>
    {% endfor %}
    
  {% endfor %}
</div>
