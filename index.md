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
  {% for b in site.BOARD %}
    {% assign key = b[0] %}
    {% assign props = b[1] %}
    {{ key }} -
    {{ props }} -
    {{b}} =b
    {% for bb in b %}{ % for bbb in bb % }
      <li><a href="{{ props.permalink }}">
        {{ props.title }}
        </a>
      {{ item[0] }} {{item[1]}}
      </li>
  {% endfor %}{% endfor %}{ % endfor % }
</ul>
+ - - 
