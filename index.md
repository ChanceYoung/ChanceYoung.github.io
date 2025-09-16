---
title: Home
---

# Hello there, I’m Chance.

I’m a software engineer, and this site is focused on improving how I explain my design approach and thought process when building projects. My passion for video games is what first drew me into software engineering, and over time I’ve had the chance to explore many facets of the field — from game development to dev operations to lightweight scripting.

Feel free to explore my project summaries below. If my work resonates with you and you think I could be a valuable addition to your team, you can download my resume [here](/assets/downloadables/ChanceYoungResume%209_3_25.pdf) or reach me at chanceyoungwebdev@gmail.com.

## Featured Projects
<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
{% assign items = site.pages %}
{% for p in items %}
  {% if p.path contains 'projects/' and p.featured == true %}
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

