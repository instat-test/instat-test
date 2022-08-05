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
<ul>
  {% for b in site.BOARD %}{% for bb in b %}{% for bbb in bb %}
    <p>{{bb}}</p>
    <p>{{bbb}}</p>
    <li><a href="{{ bbb.permalink }}">
      {{ bbb.title }}
      </a></li>
  {% endfor %}{% endfor %}{% endfor %}
</ul>
+++
