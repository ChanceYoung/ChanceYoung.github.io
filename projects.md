---
title: Projects
permalink: /projects/
---

# Projects

<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
{% assign items = site.pages | sort: "order" %}
{% for p in items %}
  {% if p.path contains 'projects/' %}
    <div class="col">
      <a class="card h-100 text-decoration-none text-light" href="{{ p.url | relative_url }}">
        <img class="card-img-top" src="{{ p.thumb | default: '/assets/images/placeholder.jpg' | relative_url }}" alt="">
        <div class="card-body">
          <h5 class="card-title mb-1">{{ p.title }}</h5>
          {% if p.summary %}<p class="card-text text-secondary small">{{ p.summary }}</p>{% endif %}
        </div>
      </a>
    </div>
  {% endif %}
{% endfor %}
</div>
