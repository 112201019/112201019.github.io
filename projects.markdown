---
layout: default
title: Projects
permalink: /projects/
---

# Projects

<div class="card-grid">
  {% for project in site.data.projects %}
    <div class="card">
      <h2>{{ project.title }}</h2>
      <p><strong>Tech Stack:</strong> {{ project.tech }}</p>
      <p>{{ project.description | markdownify }}</p>

      {% if project.github %}
        <a class="button" href="{{ project.github }}" target="_blank">GitHub</a>
      {% endif %}
      {% if project.demo %}
        <a class="button" href="{{ project.demo }}" target="_blank">Live Demo</a>
      {% endif %}
    </div>
  {% endfor %}
</div>
