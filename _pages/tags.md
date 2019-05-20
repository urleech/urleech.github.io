---
title: تگ ها
permalink: "/tags/"
layout: default
---

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tag_words = site_tags | split:',' | sort %}

<section class="blog-tags">
  <h1>تگ ها</h1>
<ul class="posts">
<!--  cycles through tag list and creates header row of all tags used in site with accompanying per-tag counts...-->
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}
    <li ><a href="#{{ this_word | cgi_escape }}" class="tag">{{ this_word }} <span>({{ site.tags[this_word].size }})</span></a></li>
  {% endunless %}{% endfor %}

<!--cycles through tag list and creates subheader for each tag name...-->
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}
  <h2 id="{{ this_word | cgi_escape }}">{{ this_word }}</h2>
<!--  lists all posts corresponding to specific tag...-->
    {% for post in site.tags[this_word] %}{% if post.title != null %}
	    <li itemscope>
      <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
      <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%Y%B%-d" }} - <i class="fas fa-clock" aria-hidden="true"></i> {% include read-time.html %}</span></p>
    </li>
    {% endif %}{% endfor %}
  {% endunless %}{% endfor %}
    </ul>
</section>
