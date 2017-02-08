---
layout: page
show_meta: false
subheadline: "Fate Core"
title: "Fair Leaves"
categories:
  - cenarios
#teaser: "Esses são alguns materiais do Destino de Perry Rhodan que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-core/Fair-Leaves/"
---


<ul>
    {% for post in site.tags.Fair-Leaves reversed %}
    <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: "<p>"  | remove: "</p>" }}</a></li>
    {% endfor %}
</ul>

## Recursos

+ [Versão para Impressão Alpha](/assets/files/FairLeavesAlpha.pdf)
+ [_Playsheets_ limpas](/assets/files/PlaysheetsFairLeaves.pdf)
+ [A Turma criada de exemplo em Fair Leaves](/assets/files/PlaysheetsFairLeavesInicial.pdf)

<ul>
