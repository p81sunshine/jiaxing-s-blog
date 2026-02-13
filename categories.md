---
layout: default
title: Categories
permalink: /categories/
---

<p>Browse posts grouped by category.</p>

{% assign grouped = site.categories | sort %}
{% for category in grouped %}
<section class="taxonomy-group">
  <h2>{{ category[0] }} ({{ category[1].size }})</h2>
  <ul class="post-list">
    {% for post in category[1] %}
    <li>
      <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
      <span class="meta-line">{{ post.date | date: "%b %-d, %Y" }}</span>
    </li>
    {% endfor %}
  </ul>
</section>
  {% endfor %}
