---
layout: default
title: Team
---

<div class="wrap">
  <h1>Il nostro team</h1>
  <div class="cards">
    {% for member in site.data.team %}
      <div class="card">
        <h3>{{ member.nome }}</h3>
        <p class="meta">{{ member.ruolo }}</p>
      </div>
    {% endfor %}
  </div>
</div>
