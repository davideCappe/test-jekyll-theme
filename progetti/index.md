---
layout: default
title: Progetti
---

<div class="wrap">
  <h1>Progetti</h1>
  <ul>
    {% for p in site.progetti %}
      <li><a href="{{ p.url }}">{{ p.title }}</a> — {{ p.excerpt | strip_html | truncate: 120 }}</li>
    {% endfor %}
  </ul>
</div>
