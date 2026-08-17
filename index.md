---
layout: default
title: Home
---

# Benvenuto

Questo è un sito di **prova**. Guarda i nostri [progetti](/progetti/).

## Ultimi articoli

{% for post in site.posts limit:3 %}

- [{{ post.title }}]({{ post.url }})
  {% endfor %}
