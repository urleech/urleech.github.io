---
title: نویسندها
permalink: "/authors/"
layout: default
---

<ul>
  {% for author in site.authors %}
    <li><a href="{{ author.url }}">{{ author.title }}</a></li>
  {% endfor %}
</ul>
