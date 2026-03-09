---
layout: default
title: Articoli
command: find ./articoli -maxdepth 1 -type f
---

# Articoli

<div class="terminal-note">
  <p>Archivio completo in formato leggibile da umani, ma organizzato come se stessi facendo inventario da shell.</p>
</div>

<div class="post-index">
{% for post in site.posts %}
  <a class="post-row" href="{{ post.url | relative_url }}">
    <span class="post-row__date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <span class="post-row__name">{{ post.slug }}.md</span>
    <span class="post-row__title">{{ post.title }}</span>
  </a>
{% endfor %}
</div>
