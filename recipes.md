---
layout: journal
title: recipes
---

{% for post in site.posts %}
  {% if post.section == "RECIPE" %}
- [{{ post.title }}]({{ post.url | relative_url }})
  {% endif %}
{% endfor %}
