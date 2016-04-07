---
layout: page
show_meta: false
subheadline: "Fate Core"
title: "Destino de Perry Rhodan"
teaser: "Esses são alguns materiais do Destino de Perry Rhodan que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
categories:
   - cenarios
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-core/perry-rhodan/"
---
<ul>
    {% for post in site.tags.Perry-Rhodan %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

