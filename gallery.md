---
layout: gallery
title: On Film, Sort Of
---

<div class="polaroids">
{% for post in site.posts %}
  {% if post.cover_image %}
    <figure>
      <a href="{{ post.url | relative_url }}">
        <img src="{{ post.cover_image | relative_url }}" alt="{{ post.title }}">
      </a>
      <figcaption>{{ post.date | date: "%b %d, %Y" }} — {{ post.title }}</figcaption>
    </figure>
  {% endif %}
{% endfor %}
</div>
