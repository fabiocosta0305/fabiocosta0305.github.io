---
layout: page
show_meta: false
subheadline: "Wearing the Cape (Playtest)"
title: "Wearing the Cape (Playtest)"
categories:
   - cenarios
permalink: "/fate-core/wtc-Playtest/"
---

{% comment %}
{{ site.tags | inspect }}
{% endcomment %}

<ul>
{% for post in site.categories.wtc %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
