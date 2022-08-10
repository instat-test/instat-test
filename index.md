---
layout: board
title: hello
description: je test
---

index here

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

{% for c in site.categories %}
  <h3>{{ c[0] }}</h3>
  ---
  <ul>
    {% for post in c[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

