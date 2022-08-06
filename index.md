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
  {%for b in site.BOARD %}
    {%assign key = b[0] %}
    {%assign props = b[1] %}
    { % for bb in b % }{ % for bbb in bb % }
    <li><a href="{{ props.permalink }}">
      {{ props.title }}
      </a></li>
  {% endfor %}{ % endfor % }{ % endfor % }
</ul>
+ - - 
