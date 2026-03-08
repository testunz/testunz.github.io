---
layout: default
title: Diario di una mente distratta
---

# Diario di una mente distratta

Sono un medico.

Per circa dieci anni ho lavorato in pronto soccorso, un luogo dove si impara rapidamente che la realtà ha poca voglia di seguire i manuali.

Oggi lavoro in medicina interna, dove il tempo scorre in modo diverso: meno caos immediato, più ragionamento, più diagnostica, più storie lunghe da ascoltare.

Molto prima della medicina, però, c’era un’altra cosa.

Il primo è stato un Commodore 64.  
Schermo blu, cursore lampeggiante, comandi BASIC digitati senza sapere davvero cosa stessi facendo, ma con la sensazione molto chiara che lì dentro ci fosse qualcosa di importante.

Da allora non ho mai smesso.

Questo spazio è un posto semplice dove raccolgo pensieri sparsi, esperimenti e deviazioni mentali.

A volte parlerò di medicina.  
A volte di tecnologia.  
A volte di Linux, server domestici, AI o piccoli progetti inutilmente complicati.

Altre volte saranno solo appunti di viaggio di una mente che si distrae facilmente.

## Articoli

{% for post in site.posts limit:10 %}
[{{ post.date | date: "%Y-%m-%d" }}] [{{ post.slug }}.md]({{ post.url }})
{% endfor %}
