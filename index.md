---
title: Home
---

# Hey, I’m Chance 👋
I build practical software (ERP integrations, automation) and small finished games.  
This site is a **project-summary** library: more detail than a résumé, less than a full repo.

## Featured Projects
<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
{% assign items = site.pages | sort: "order" %}
{% assign shown = 0 %}
{% for p in items %}
  {% if p.path contains 'projects/' and p.featured == true and shown < 6 %}
    <div class="col">
      <a class="card h-100 text-decoration-none text-light" href="{{ p.url | relative_url }}">
        <img class="card-img-top" src="{{ p.thumb | default: '/assets/images/placeholder.jpg' | relative_url }}" alt="">
        <div class="card-body">
          <h5 class="card-title mb-1">{{ p.title }}</h5>
          {% if p.summary %}<p class="card-text text-secondary small">{{ p.summary }}</p>{% endif %}
        </div>
      </a>
    </div>
    {% assign shown = shown | plus: 1 %}
  {% endif %}
{% endfor %}
</div>

<p class="mt-3"><a class="btn btn-outline-light" href="{{ '/projects/' | relative_url }}">View all projects</a></p>
