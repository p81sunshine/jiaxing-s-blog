---
layout: default
title: Tags
permalink: /tags/
---

<p>Browse posts grouped by tag.</p>

{% assign grouped = site.tags | sort %}
{% for tag in grouped %}
<section class="taxonomy-group">
  <h2>#{{ tag[0] }} ({{ tag[1].size }})</h2>
  <ul class="post-list">
    {% for post in tag[1] %}
    <li>
      <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
      <span class="meta-line">{{ post.date | date: "%b %-d, %Y" }}</span>
    </li>
    {% endfor %}
  </ul>
</section>
  {% endfor %}
