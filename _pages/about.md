---
title: درباره
permalink: "/about/"
layout: page
---

<!--<head>
<style>
h1 {
    font-size: 4rem;
}
</style>
</head>
<div class="soc">
		<a href="https://instagram.com/kaubosh" target="_blank" title="اینستاگرام" ><i class="fab fa-instagram"></i></a>
		<a href="https://www.pinterest.com/kaubosh/" target="_blank" title="پینترست" ><i class="fab fa-pinterest"></i></a>
        <a href="https://twitter.com/intent/user?screen_name=kaubosh" target="_blank" title="توییتر" ><i class="fab fa-twitter"></i></a>
        <a href="https://rawg.io/@kaubosh/games" target="_blank" title="راوگ" ><i class="fas fa-registered"></i></a>
        <a href="https://t.me/kaubosh" target="_blank" title="تلگرام" ><i class="fab fa-telegram"></i></a>
        <a href="https://leagueofcomicgeeks.com/profile/kaubosh/read-list" target="_blank" title="لیگ آو کامیک گیکز" ><i class="fi-lcg"></i></a>
        <a href="https://kitsu.io/users/KauBosh/library" target="_blank" title="کیتسو" ><i class="fi-kit"></i></a>
        <a href="http://goodreads.com/kaubosh" target="_blank" title="گودریدز" ><i class="fab fa-goodreads"></i></a>
        <a href="https://www.last.fm/user/KauBosh" target="_blank" title="لست.اف ام" ><i class="fab fa-lastfm-square"></i></a>
        <a href="https://trakt.tv/users/kaubosh/" target="_blank" title="واچ لیست سریال و فیلم ها" ><i class="fi-trk"></i></a>
        <a href="https://open.spotify.com/user/uchuuv8r0dwwmp6orppsy5el7/playlist/1Y5H4fXushydlVeuIpPgIc" target="_blank" title="پلی لیست اسپاتیفای" ><i class="fab fa-spotify"></i></a>
		<a href="https://tinyletter.com/kaubosh" target="_blank" title="خبرنامه" ><i class="fas fa-envelope"></i></a>
		<a href="https://ownetic.com/@kaubosh" target="_blank" title="خبرنامه" ><i class="fas fa-genderless fa-lg"></i></a>
		<a href="{{ ROOT }}atom.xml" target="_blank" title="خبرنامه" ><i class="fas fa-rss-square"></i></a>
</div>-->
<div class="small-wrapper">
  <div class="about-container">
    <section class="about-header">
      <div class="author-image-container">
        <img src="{{site.baseurl}}/assets/img/{% if site.author-pic %}{{site.author-pic}}{% endif %}" alt="{{site.author}}">
      </div>
      <p class="subtitle">{{site.about-author}}</p>
    </section>
    <section class="about-body">
      <ul class="contact-list">
      {% if site.email %}
        <li class="email"><a href="mailto:{{site.email}}"><i class="fa fa-envelope-o"></i></a></li>
      {% else %}
        <li class="email"><a href="mailto:example.adam@blog.com"><i class="fa fa-envelope-o" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.phone %}
        <li class="phone"><a href="tel:{{site.phone}}"><i class="fa fa-phone"></i></a></li>
      {% else %}
        <li class="phone"><a href="tel:+98910000000"><i class="fa fa-phone" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.website %}
        <li class="website"><a href="http://{{site.website}}" target="_blank"><i class="fa fa-globe"></i></a></li>
      {% else %}
        <li class="website"><a href="https://LuciferiusBlaze.github.io" target="_blank"><i class="fa fa-globe" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.linkedin %}
        <li class="linkedin"><a href="https://in.linkedin.com/in/{{site.linkedin}}" target="_blank"><i class="fa fa-linkedin"></i></a></li>
      {% else %}
        <li class="linkedin"><a href="https://in.linkedin.com/" target="_blank"><i class="fa fa-linkedin" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.github %}
        <li class="github"><a href="http://github.com/{{site.github}}" target="_blank"><i class="fa fa-github"></i></a></li>
      {% else %}
        <li class="github"><a href="http://github.com/LuciferiusBlaze" target="_blank"><i class="fa fa-github" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.twitter %}
        <li class="twitter"><a href="https://twitter.com/{{site.twitter}}" target="_blank"><i class="fa fa-twitter"></i></a></li>
      {% else %}
        <li class="twitter"><a href="https://twitter.com/LuciferiusBlaze" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.facebook %}
        <li class="facebook"><a href="https://facebook.com/{{site.facebook}}" target="_blank"><i class="fa fa-facebook"></i></a></li>
      {% else %}
        <li class="facebook"><a href="https://facebook.com/LuciferiusBlaze" target="_blank"><i class="fa fa-facebook" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.instagram %}
        <li class="instagram"><a href="https://instagram.com/{{site.instagram}}" target="_blank"><i class="fa fa-instagram"></i></a></li>
      {% else %}
        <li class="instagram"><a href="https://instagram.com/LuciferiusBlaze" target="_blank"><i class="fa fa-instagram" aria-hidden="true"></i></a></li>
      {% endif %}

      {% if site.pinterest %}
        <li class="pinterest"><a href="https://pinterest.com/{{site.pinterest}}" target="_blank"><i class="fa fa-pinterest"></i></a></li>
      {% else %}
        <li class="pinterest"><a href="https://pinterest.com/LuciferiusBlaze" target="_blank"><i class="fa fa-pinterest" aria-hidden="true"></i></a></li>
      {% endif %}
      </ul>
    </section> <!-- End About Body-->
  </div> <!-- End About Container -->
</div> <!-- End Small Wrapper -->