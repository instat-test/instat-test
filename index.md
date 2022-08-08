---
layout: default
lang: ru-RU
title: hello
description: je test
---

content here

<ul class="entries">
  {% for post in site.posts %}
 
  <li>
    <a href="{{ post.url }}">
      <p>{{ post.title }}</p>
    </a>
  </li>
 
  {% endfor %}
</ul>
- - -
<!-- https://github.com/shopify/liquid/wiki/liquid-for-designers -->
<ul>
  {% for b in site.data.boards %}
    {% assign props = b[1] %}
    {% if props contains 'disable' %}
      {% continue %}
    {% endif %}
      <li><a href="{{ props.permalink }}">
        props {{ props.title }}
        </a>
      </li>
  {% endfor %}
</ul>
++ - - 
