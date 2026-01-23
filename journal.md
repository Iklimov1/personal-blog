---
layout: journal
title: journal
---

{% for post in site.posts %}
{% if post.section == "LIFE" %}

- **{{ post.date | date: "%b %d" }}** — [{{ post.title }}]({{ post.url | relative_url }})
  {% endif %}
  {% endfor %}
