---
layout: page
show_meta: false
title: "Personagens exemplos"
permalink: "/personagens/"
---

<h2>Alguns personagens exemplo</h2>

{% assign ptposts = site.categories.personagens | where: 'language','br' | sort: "title" %}
{% assign enposts = site.categories.personagens | where: 'language','en' | sort: "title" %}

{% assign pt_sorted_posts = ptposts | group_by: "tags"  | sort: "name"  %}

{% for post_tag in pt_sorted_posts %}

<h3>{{ post_tag.name | remove: '[' | remove: ']' | remove: '"' }}</h3>

<ul>
{% for mypost in post_tag.items %}
<li><a href="{{ mypost.url }}">{{ mypost.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
{% endfor %}
</ul>

{% endfor %}

{% comment %}
{% capture site_tags %}{% for post in site.categories.personagens %}{% for tag in post.tags %}{{ tag }},{% endfor %}{% endfor %}
{% endcapture %}

{% assign tag_words = site_tags | split:',' | sort %}
{% assign tags = tag_words[1] %}

{% for item in tag_words %}
    {% unless tags contains item %}
        {% capture tags %}{{ tags }}|{{ item }}{% endcapture %}
    {% endunless %}
{% endfor %}

{% assign final_tags = tags  | split: '|' %}

{% for tag in final_tags %}
<ul>
<li> <h3>{{ tag }}</h3> </li>
<ul>
{% for mypost in ptposts  %}
{% if mypost.tags contains tag %}
<li><a href="{{ mypost.url }}">{{ mypost.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
{% endif %}
{% endfor %}
</ul>
{% endfor %}
</ul>
{% endcomment %}


<h2>Some sample characters</h2>

{% assign en_sorted_posts = enposts | group_by: "tags"  | sort: "name"  %}

{% for post_tag in en_sorted_posts %}

<h3>{{ post_tag.name | remove: '[' | remove: ']' | remove: '"' }}</h3>

<ul>
{% for mypost in post_tag.items %}
<li><a href="{{ mypost.url }}">{{ mypost.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
{% endfor %}
</ul>

{% endfor %}

{% comment %}

Apenas para referência de código

{% capture site_tags %}{% for post in site.categories.personagens %}{% for tag in post.tags %}{{ tag }},{% endfor %}{% endfor %}
{% endcapture %}
    
<!-- `tag_words` is a sorted array of the tag names. -->
{% assign tag_words = site_tags | split:',' | sort %}
{% assign tags = tag_words[1] %}

{% for item in tag_words %}
    {% unless tags contains item %}
        {% capture tags %}{{ tags }}|{{ item }}{% endcapture %}
    {% endunless %}
{% endfor %}

{{ tag_words }} 

{{ tags }}

{% endcomment %}
