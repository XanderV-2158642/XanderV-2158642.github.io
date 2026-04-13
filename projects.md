---
layout: page
title: Projects
permalink: /projects/
---

Here are some of the projects I've been working on:

<div class="projects-grid">
{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}

  <a href="{{ project.url | relative_url }}" class="project-card">
    {% if project.image %}
    <div class="project-image">
      <img src="{{ project.image }}" alt="{{ project.title }}">
    </div>
    {% endif %}
    <div class="project-info">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <span class="project-tech">{{ project.technologies | join: ", " }}</span>
    </div>
  </a>

{% endfor %}
</div>
