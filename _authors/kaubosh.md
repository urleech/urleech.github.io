---
layout: default
title: کاوبوش
permalink: /kaubosh/
---

dvfd


<h1 class="">{{ page.title }}</h1>
<div class="bio">{{ page.content }}</div>

{% assign posts = site.posts | where: 'author', page.title %}
{% for post in posts %}
  {% include post.html %}
{% endfor %}