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
    b0{{ b[0] }}
    b1{{ b[1] }}
    item0 {{ item[0] }}
    item1 {{ item[1] }}
    {% assign props = b[1] %}
    props {{props}}
    { % for bb in b[1] % }{ % for bbb in bb % }
      <li><a href="{{ props.permalink }}">
        props {{ props.title }}
        </a>
      bb {{ item[0] }} == {{item[1]}}
      </li>
    { % endfor % }
  {% endfor %}
</ul>
+ - - 
