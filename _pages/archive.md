---
title: آرشیو
permalink: "/archive/"
layout: page
---

<ul class="posts">
  {% for post in site.posts %}

    {% unless post.next %}
      <h3>{{ post.date | date: '%Y' }}</h3>
    {% else %}
      {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
      {% if year != nyear %}
        <h3><!--{{ post.date | date: '%Y' }}--><time id="date:{{post.date}}"></time>
        <script>
            var date='{{post.date}}'
            moment.loadPersian(true);
            var mom = moment(date, 'YYYY-M-D HH:mm:ss TZD').format('jYYYY');
            document.getElementById("date:{{post.date}}").innerText=mom
        </script></h3>
      {% endif %}
    {% endunless %}

    <li itemscope>
      <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
      <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> <!--{{ post.date | date: "%B %-d" }}--><time id="date:{{post.date}}"></time>
        <script>
            var date='{{post.date}}'
            moment.loadPersian(true);
            var mom = moment(date, 'YYYY-M-D HH:mm:ss TZD').format('jD jMMMM jYYYY');
            document.getElementById("date:{{post.date}}").innerText=mom
        </script> - <i class="fas fa-clock" aria-hidden="true"></i> {% include read-time.html %}</span></p>
    </li>

  {% endfor %}
</ul>
