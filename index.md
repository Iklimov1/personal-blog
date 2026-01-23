---
layout: default
title: Home
---

# Welcome

Recent posts:

{% for post in site.posts %}

- [{{ post.title }}]({{ post.url }}) — {{ post.section }} · {{ post.vibe }}
  {% endfor %}
