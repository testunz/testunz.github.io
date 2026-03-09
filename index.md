---
layout: default
title: Diario di una mente distratta
---

<section class="home-intro">
  <p>Sono un medico. Uno Pneumologo.</p>

  <p>Prestato per dieci anni al pronto soccorso, un luogo dove realtà e immaginazione si fondono nello spazio tempo infinito di un turno.</p>

  <p>Oggi lavoro in medicina interna, dove invece il tempo scorre in modo diverso. Meno caos immediato, più ragionamento, più diagnostica, più cose da spulciare, roba nuova da imparare, carne viva.</p>

  <p>Molto prima della medicina, però, c'è stato lui.</p>

  <p>Il primo è stato un C64.<br>
  Schermo blu, cursore lampeggiante, comandi BASIC digitati senza sapere davvero cosa stessi facendo, ma con la sensazione molto chiara che lì dentro ci fosse qualcosa di importante da capire, da smontare.</p>

  <p>Da allora non ho più smesso.</p>

  <p>Questo spazio è un posto semplice dove raccolgo pensieri sparsi, esperimenti e deviazioni mentali.</p>

  <p>A volte parlerò di medicina.<br>
  A volte di tecnologia.<br>
  A volte di Linux, server domestici, AI o piccoli progetti inutilmente complicati, che ti rubano le notti.</p>

  <p>Altre volte saranno solo appunti di viaggio di una mente che si distrae facilmente.</p>
</section>

<section class="home-feed">
  <div class="section-heading">
    <h2>Ultimi articoli</h2>
    <p>Nuovi post, esperimenti e appunti in ordine cronologico.</p>
  </div>

  <div class="post-list">
    {% for post in site.posts limit:10 %}
      <article class="post-card">
        <p class="post-card-meta">{{ post.date | date: "%d %B %Y" }}</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | normalize_whitespace | truncate: 180 }}</p>
        <a class="post-card-link" href="{{ post.url | relative_url }}">Apri articolo -></a>
      </article>
    {% endfor %}
  </div>
</section>
