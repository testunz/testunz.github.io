---
layout: default
title: Articoli
---

<section class="archive-page">
  <div class="section-heading">
    <h1>Archivio articoli</h1>
    <p>Tutti i post pubblicati, in ordine dal più recente al più vecchio.</p>
  </div>

  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-card">
        <p class="post-card-meta">{{ post.date | date: "%d %B %Y" }}</p>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt | strip_html | normalize_whitespace | truncate: 220 }}</p>
        <a class="post-card-link" href="{{ post.url | relative_url }}">Leggi il post -></a>
      </article>
    {% endfor %}
  </div>
</section>
