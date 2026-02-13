---
layout: default
title: Home
---

<p class="home-intro">
  Hi, I am Jiaxing. I write about large language model, software engineering, thinking, and personal workflows.
</p>

<p>
  <a href="{{ '/about/' | relative_url }}">About me</a> ·
  <a href="{{ '/posts/' | relative_url }}">All posts</a> ·
  <a href="{{ '/categories/' | relative_url }}">Categories</a> ·
  <a href="{{ '/tags/' | relative_url }}">Tags</a>
</p>

## Recent posts

<ul class="post-list">
  {% for post in site.posts limit:8 %}
  <li>
    <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
    <span class="meta-line">{{ post.date | date: "%b %-d, %Y" }}</span>
  </li>
  {% endfor %}
</ul>
