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
      <img src="{{ post.image }}" />
      <h3>{{ post.title }}</h3>
    </a>
  </li>
 
  {% endfor %}
</ul>

