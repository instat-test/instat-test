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
::
{% for ind in site.BOARD %}
    <a href="{{ site.BOARD[ind].permalink }}">
      {{ind}} {{ site.BOARD[ind].title }}
    </a>
{% endfor %}
::
