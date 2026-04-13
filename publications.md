---
layout: page
title: Publications
permalink: /publications/
---

Here are my publications:

<div class="pubs-list">
{% assign sorted_publications = site.publications | sort: 'date' | reverse %}
{% for pub in sorted_publications %}
<div class="pub-item-full">
  <h3><a href="{{ pub.url | relative_url }}">{{ pub.title }}</a>{% if pub.award %} <span class="award-badge">{{ pub.award }}</span>{% endif %}</h3>
  <p class="pub-meta">{{ pub.conference }} • {{ pub.date | date: "%Y" }}{% if pub.author_role %} • <span class="author-role">{{ pub.author_role }}</span>{% endif %}</p>
  <p>{{ pub.description }}</p>
  {% if pub.image %}<p class="pub-links"><a href="{{ pub.image }}">Poster</a> • <a href="{{ pub.url | relative_url }}">Read More</a></p>{% else %}<p class="pub-links"><a href="{{ pub.url | relative_url }}">Read More</a></p>{% endif %}
</div>
{% endfor %}
</div>