---
layout: page
title: Projects
permalink: /projects/
---

Here are some of the projects I've been working on:

{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}

## [{{ project.title }}]({{ project.url | relative_url }})

{{ project.description }}

**Technologies:** {{ project.technologies | join: ", " }}

{% if project.github %}[GitHub]({{ project.github }}){% endif %}{% if project.demo %} • [Demo]({{ project.demo }}){% endif %} • [Read More]({{ project.url | relative_url }})

---
{% endfor %}
