---
permalink: /pics/
title: "Pics"
layout: splash
header:
  image: /assets/images/landpage-header.png
classes: wide
assets_folder: /assets/posters/
---


{% for poster in site.data.posters %}

  <div style="float:left;margin: 5px">
    <div>
      <span style="font-size:0.7em;font-weight: bold;"><i class="fas fa-fw fa-tags" aria-hidden="true"></i>&nbsp;{{ poster.category }}</span><br>
      <a href="{{site.baseurl}}{{page.assets_folder}}{{poster.image}}" target="_blank" class=".btn .btn--success .btn--large">
        <img src="{{site.baseurl}}{{page.assets_folder}}{{poster.thumbnail}}" alt="{{poster.description}}">
      </a>
    <!-- w300 A4 -->
    </div>
  </div>


{% endfor %}
