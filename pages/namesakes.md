---
layout: page
show_meta: false
subheadline: "Namesakes"
title: "Namesakes"
teaser: "Esses são alguns materiais de Namesakes que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
categories:
   - cenarios
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-core/namesakes/"
---
<ul>
    {% for post in site.tags.namesakes %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
