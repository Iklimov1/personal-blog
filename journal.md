---
layout: journal
title: journal
---

{% for post in site.posts %}
- **{{ post.date | date: "%b %d" }}** — [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
