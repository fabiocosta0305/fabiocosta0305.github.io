---
layout: page
show_meta: false
subheadline: "RPG"
title: "Meus Materiais de RPG!"
teaser: "Esses são alguns materiais de RPG que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
permalink: "/rpg/"
---

Materias de RPG que Escrevi com o tempo

<ul>
    {% for post in site.tipos %}
    <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
    {% comment %}
    {{ post.content }}
    {% endcomment %}
    {% endfor %}
</ul>
