---
title: Home
---

# Hello there, I’m Chance.

I’m a software engineer, and this site is focused on improving how I explain my design approach and thought process when building projects. My passion for video games is what first drew me into software engineering, and over time I’ve had the chance to explore many facets of the field — from game development to dev operations to lightweight scripting.

Feel free to explore my project summaries below. If my work resonates with you and you think I could be a valuable addition to your team, you can view my resume [here](/assets/downloadables/ChanceYoungResume%209_3_25.pdf), download it with the nav link, or reach me directly at <chanceyoungwebdev@gmail.com>.

## Featured Projects
<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
{% for project in site.projects %}
  {% if project.featured == true %}
    <div class="col">
      <a class="card h-100 text-decoration-none text-light" href="{{ project.url | relative_url }}">
        <img class="card-img-top" src="{{ project.thumb | default: '/assets/images/placeholder.jpg' | relative_url }}" alt="">
        <div class="card-body">
          <h5 class="card-title mb-1">{{ project.title }}</h5>
          {% if project.summary %}<p class="card-text text-secondary small">{{ project.summary }}</p>{% endif %}
        </div>
      </a>
    </div>
  {% endif %}
{% endfor %}
</div>

