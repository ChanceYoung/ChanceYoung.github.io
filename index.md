---
title: Home
layout: default
---

# Hey, I’m Chance
Short sentence on what you do (ERP integrations, automation, indie games).
Add 1–2 links if you want (GitHub, LinkedIn).

## Latest posts
<div class="post-grid">
{% for post in site.posts limit:9 %}
  <a class="post-card" href="{{ post.url | relative_url }}">
    {% assign thumb = post.thumb | default: '/assets/images/placeholder.jpg' %}
    <img class="post-thumb" src="{{ thumb | relative_url }}" alt="">
    <div class="post-body">
      <h3 class="post-title">{{ post.title }}</h3>
      <div class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</div>
    </div>
  </a>
{% endfor %}
</div>
