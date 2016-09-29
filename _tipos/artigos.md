---
layout: page
show_meta: false
subheadline: "Artigos"
title: "Meus Artigos e reviews!"
permalink: "/artigos/"
---

Artigos que escrevi ou traduzi
        
<ul>
    {% for post in site.tags.Artigos %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

Reviews que escrevi

<ul>
    {% for post in site.categories.reviews %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
