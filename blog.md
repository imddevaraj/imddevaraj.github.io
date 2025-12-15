---
layout: default
title: Blog
permalink: /blog/
---

<div class="container" style="padding-top: 4rem;">
  <h1 class="section-title" style="margin-top: 0;">Latest Thoughts</h1>
  
  <ul class="post-list">
    {% for post in site.posts %}
    <li class="post-item">
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    </li>
    {% endfor %}
  </ul>
</div>
