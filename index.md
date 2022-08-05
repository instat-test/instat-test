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
+++
<ul>
  {% for bbb in site.BOARD %}
    {% for b in bbb %}
    <li><a href="{{ b.permalink }}">
      {{ b.title }}
      </a></li>
    {% endfor %}
  {% endfor %}
</ul>
+++
