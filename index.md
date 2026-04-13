---
layout: home
permalink: /
title: ""
---

# {{site.title}}

## About Me

Computer science student that started coding in 2020. Passionate about Computational fabrication and CyberSecurity. Currently focused on LLMs and small electronics. 


## Publications

{% assign sorted_publications = site.publications | sort: 'date' | reverse %}
{% for pub in sorted_publications %}
<div class="pub-item">
  <h3><a href="{{ pub.url | relative_url }}">{{ pub.title }}</a>{% if pub.award %} <span class="award-badge">{{ pub.award }}</span>{% endif %}</h3>
  <p class="pub-meta">{{ pub.conference }} • {{ pub.date | date: "%Y" }}</p>
  <p>{{ pub.description }}</p>
  <p class="pub-links">{% if pub.image %}<a href="{{ pub.image }}">Paper PDF</a> • {% endif %}<a href="https://dl.acm.org/doi/10.1145/3772318.3791414">ACM</a></p>
</div>
{% endfor %}


## Featured Projects

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

[View All Projects →](/projects/)


## Experience

<div class="experience-list">

<div class="experience-item">
  <div class="exp-header">
    <h3>Summer internship</h3>
    <span class="exp-date">14/07/2025 - 12/09/2025</span>
  </div>
  <p class="exp-company">Digital Future Lab (previously EDM) | Intern</p>
  <ul class="exp-tasks">
    <li>Creating visuals/dashboard UI's to enhance the training process of students learning Craft skills</li>
    <li>Use of LLM's, Unity game engine, and python for machine learning</li>
  </ul>
</div>

<div class="experience-item">
  <div class="exp-header">
    <h3>Summer internship</h3>
    <span class="exp-date">01/07/2024 - 14/08/2024</span>
  </div>
  <p class="exp-company">Expertisecentrum digitale media (EDM) | Intern</p>
  <ul class="exp-tasks">
    <li>Creating AR interfaces to show student executions of a craft skill in 3d and their performance</li>
    <li>Working with the MagicLeap2, and virtual reality paradigms</li>
    <li>Machine learning in python</li>
    <li>My work was featured at the release of the new Digital Future Lab, and was also covered on <a href="https://www.tvl.be/nieuws/80-onderzoekers-werken-aan-digitale-toekomst-in-digital-future-lab-van-uhasselt-174428" target="_blank">local news</a></li>
  </ul>
</div>

<div class="experience-item">
  <div class="exp-header">
    <h3>Full stack development</h3>
    <span class="exp-date">01/07/2023 - 31/12/2024</span>
  </div>
  <p class="exp-company">Bogie lab | Student programmer</p>
  <ul class="exp-tasks">
    <li>Development of a management system used at BogieLab, to reduce the breeding of testing animals</li>
    <li>Full stack development using Ruby on Rails and React</li>
    <li>Cloud deployment using Google Cloud</li>
  </ul>
</div>

</div>


## Education

<div class="education-list">

<div class="education-item">
  <h3>Master of Science in Computer Science</h3>
  <p class="edu-school">Hasselt University | Expected Graduation: June 2026</p>
  <p class="edu-details"><strong>Relevant Coursework:</strong> Human Computer interaction, Networking and security, AI and machine learning</p>
  <p class="edu-details"><strong>Weighted average:</strong> 80%</p>
</div>

<div class="education-item">
  <h3>Bachelor of Computer Science</h3>
  <p class="edu-school">Hasselt University | Graduation: September 2024</p>
  <p class="edu-details"><strong>Achievements:</strong> Cum Laude</p>
</div>

</div>