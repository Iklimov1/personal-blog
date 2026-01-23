---
layout: home
title: Home
---

# Welcome

Recent posts:

{% for post in site.posts %}

- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.section }} · {{ post.vibe }}
  {% endfor %}
