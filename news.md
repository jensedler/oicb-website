---
layout: default
title: "News & Events"
---
<h1>News & Events</h1>
<ul>
{% for post in site.news %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d.%m.%Y" }}</time>
  </li>
{% endfor %}
</ul>