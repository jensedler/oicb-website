---
layout: default
title: "Team"
---
<h1>Team</h1>
<div class="team-grid">
{% for member in site.data.team %}
  <figure data-aos="fade-up">
    <img src="{{ '/assets/img/' | append: member.photo | relative_url }}" alt="{{ member.name }}" />
    <figcaption>
      <strong>{{ member.name }}</strong><br>
      {{ member.role }}
    </figcaption>
  </figure>
{% endfor %}
</div>