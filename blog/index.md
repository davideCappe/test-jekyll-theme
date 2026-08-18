---
layout: default
title: Blog
---

<div class="wrap">
  <h1>Blog</h1>
  <div class="cards">
    {% for post in site.posts %}
      <article class="card">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="meta">{{ post.date | date: "%d %B %Y" }}</p>
        <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
      </article>
    {% endfor %}
  </div>
</div>
