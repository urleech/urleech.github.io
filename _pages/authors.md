---
layout: default
title: نویسندها
permalink: /authors/
---

<ul>
  {% for author in site.authors %}
    <li><a href="{{ author.url }}">{{ author.title }}</a></li>
  {% endfor %}
</ul>
