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
    !! {{b}} =b
    {% for bb in b %}{ % for bbb in bb % }
      <li><a href="{{ props.permalink }}">
        props {{ props.title }}
        </a>
      bb {{ bb[0] }} == {{bb[1]}}
      </li>
    {% endfor %}
  {% endfor %}
</ul>
+ - - 
