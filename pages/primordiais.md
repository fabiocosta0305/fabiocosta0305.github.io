---
layout: page
show_meta: false
subheadline: "Fate Core"
title: "Primordiais"
categories:
  - cenarios
teaser: "Alguns materiais antigos do meu antigo cenário de Espírito do Século, Primordiais, que agora estou readaptando para Fate core"
permalink: "/fate-core/Primordiais/"        
---

Alguns materiais antigos do meu antigo cenário de Espírito do Século, Primordiais, que agora estou readaptando para Fate core


<ul>
<li> Materiais em Geral
<ul>
    {% for post in site.tags.Primordiais %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
<li> Materias para <i>Espírito do Século (Fate 3.0)</i>
<ul>
    {% for post in site.posts %}
    {% if post.tags contains "Primordiais (Espírito do Século)" %}
                  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}                  
    {% endfor %}
</ul>
<li> Materias para <i>Fate Básico</i>
<ul>
    {% for post in site.posts %}
    {% if post.tags contains "Primordiais (Fate Básico)" %}
                  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}                  
    {% endfor %}
</ul>
<ul>
