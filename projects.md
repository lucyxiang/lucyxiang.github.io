---
layout: default
title: Projects
---

# Projects

{% for project in site.projects %}
<div class="project-card">
  {% if project.image %}
  <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
  {% endif %}
  <h2>{{ project.title }}</h2>
  <p>{{ project.description }}</p>
  <a href="{{ project.github }}" class="project-link">View on GitHub</a>
</div>
{% endfor %}
