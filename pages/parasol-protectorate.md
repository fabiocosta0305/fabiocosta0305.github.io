---
layout: page
show_meta: false
subheadline: "Destino do Protetorado da Sombrinha"
title: "Protetorado da Sombrinha"
teaser: "Esses são alguns materiais do Protetorado da Sombrinha que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
categories:
   - cenarios
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-core/parasol-protectorate/"
---
<ul>
    {% for post in site.tags.Parasol-Protectorate %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
