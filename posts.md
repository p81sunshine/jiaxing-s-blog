---
layout: default
title: Posts
permalink: /posts/
---

<p>This is the full archive in reverse chronological order.</p>

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
    <span class="meta-line">{{ post.date | date: "%b %-d, %Y" }} · {{ post.categories | join: ", " }}</span>
  </li>
  {% endfor %}
</ul>
