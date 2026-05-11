---
layout: default
title: Home
---

## Latest Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      {% if post.theme %}
      <p class="post-theme">Theme: {{ post.theme }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
