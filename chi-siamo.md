---
layout: default
title: Chi siamo
---

# Il team

{% for persona in site.data.team %}

- **{{ persona.nome }}** — {{ persona.ruolo }}
  {% endfor %}
