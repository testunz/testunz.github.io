---
layout: default
title: Diario di una mente distratta
command: ./bootstrap --profile diario
---

# Diario di una mente distratta

<div class="terminal-note">
  <p>medico in medicina interna, ex pronto soccorso, curioso cronico davanti a ogni cursore lampeggiante.</p>
</div>

Sono un medico. Uno pneumologo.

Per dieci anni sono stato in pronto soccorso, un posto dove realtà e immaginazione si mischiano nello spazio-tempo infinito di un turno. Oggi lavoro in medicina interna: meno impatto immediato, più ragionamento, più diagnostica, più materiale da smontare e capire.

Molto prima della medicina, però, c'è stato un monitor blu con un cursore che lampeggiava.

Il primo computer è stato un C64. Comandi BASIC digitati senza sapere bene cosa stessi facendo, ma con la sensazione chiarissima che lì dentro ci fosse qualcosa di importante da capire e smontare.

Da allora non ho più smesso.

Questo blog raccoglie pensieri sparsi, esperimenti e deviazioni mentali. Niente branding pulito, niente cartoline: solo output, file aperti, note prese al volo.

## Cosa passa da qui

- medicina pratica e ragionata
- Linux, server di casa, automazioni, AI
- progetti inutilmente complicati che meritano comunque di esistere
- appunti veloci di una mente facilmente distraibile

## Ultimi file aperti

<div class="command-block">
  <div class="inline-command">ls -lt ~/articoli | head</div>
  <div class="post-index post-index--compact">
  {% for post in site.posts limit: 8 %}
    <a class="post-row" href="{{ post.url | relative_url }}">
      <span class="post-row__date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <span class="post-row__name">{{ post.slug }}.md</span>
      <span class="post-row__title">{{ post.title }}</span>
    </a>
  {% endfor %}
  </div>
</div>
