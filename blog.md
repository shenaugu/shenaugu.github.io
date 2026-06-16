---
layout: page
title: Notes
subtitle: Research log, paper notes, and things I'm figuring out
permalink: /blog/
---

A working notebook — short write-ups of experiments, papers I'm reading, and ideas I want
to remember. Rough by design.

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {% if post.excerpt %}<p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 28 }}</p>{% endif %}
    </li>
  {% endfor %}
</ul>
