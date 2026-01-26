---
layout: journal
title: journal
---

<ul>
{% for post in site.posts %}
  {% if post.section == "journal" %}
    <li>
      <strong>{{ post.date | date: "%b %d" }}</strong> — <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>
