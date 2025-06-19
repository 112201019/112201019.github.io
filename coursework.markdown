---
layout: default
title: Coursework
permalink: /coursework/
---

#  Coursework


##  Core CS Courses

<ul>
  {% for item in site.data.coursework.core %}
    <li>{{ item }}</li>
  {% endfor %}
</ul>


##  Electives & Advanced Topics

<ul>
  {% for item in site.data.coursework.electives %}
    <li>{{ item }}</li>
  {% endfor %}
</ul>


##  Projects Done in Coursework

{% for p in site.data.coursework.projects %}
<div class="card">
  <h3>{{ p.title }}</h3>
  <p><strong>Course:</strong> {{ p.course }}</p>
  <p>{{ p.desc }}</p>
</div>
{% endfor %}
