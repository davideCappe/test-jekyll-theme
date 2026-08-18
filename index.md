---
layout: default
title: Home
---

<section class="hero">
  <div class="wrap">
    <h1>Benvenuto su {{ site.title }}</h1>
    <p>{{ site.description }}</p>
    <p><a class="btn" href="{{ '/progetti/' | relative_url }}">Scopri i progetti</a></p>
  </div>
</section>

<section class="latest wrap">
  <h2>Ultimi articoli</h2>
  <div class="cards">
    {% for post in site.posts limit:3 %}
    <article class="card">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="meta">{{ post.date | date: "%d %B %Y" }} • {% for t in post.tags %}<span class="tag">{{ t }}</span>{% endfor %}</p>
      <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
    </article>
    {% endfor %}
  </div>
</section>

<section class="wrap">
  <h2>Progetti in evidenza</h2>
  <ul class="projects">
    {% for p in site.progetti limit:3 %}
      <li><a href="{{ p.url }}">{{ p.title }}</a></li>
    {% endfor %}
  </ul>
</section>
