---
layout: default
title: Diario di una mente distratta
---

# Diario di una mente distratta

Sono un medico. Uno Pneumologo.

Prestato per dieci anni al pronto soccorso, un luogo dove realtà e immaginazione si fondono nello spazio tempo infinito di un turno.

Oggi lavoro in medicina interna, dove invece il tempo scorre in modo diverso. Meno caos immediato, più ragionamento, più diagnostica, più cose da spulciare, roba nuova da imparare, carne viva. 

Molto prima della medicina, però, c’è stato lui.

Il primo è stato un C64.  
Schermo blu, cursore lampeggiante, comandi BASIC digitati senza sapere davvero cosa stessi facendo, ma con la sensazione molto chiara che lì dentro ci fosse qualcosa di importante da capire, da smontare.

Da allora non ho più smesso.

Questo spazio è un posto semplice dove raccolgo pensieri sparsi, esperimenti e deviazioni mentali.

A volte parlerò di medicina.  
A volte di tecnologia.  
A volte di Linux, server domestici, AI o piccoli progetti inutilmente complicati, che ti rubano le notti.

Altre volte saranno solo appunti di viaggio di una mente che si distrae facilmente.

## Articoli

{% for post in site.posts limit:10 %}
[{{ post.date | date: "%Y-%m-%d" }}] [{{ post.slug }}.md]({{ post.url }})
{% endfor %}
