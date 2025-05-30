---
layout: default
title: "Projekte"
---
<h1>Projekte</h1>
<ul>
{% for project in site.data.projects %}
  <li>
    <h2>{{ project.title }}</h2>
    <p>{{ project.teaser }}</p>
  </li>
{% endfor %}
</ul>