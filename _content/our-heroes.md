---
layout: basic
permalink: "/our-heroes/"
title: Our heroes
status: published
imgBanner: /assets/images/pages/
imgThumbnail: /assets/images/pages/
---

<div class="row small-up-2 medium-up-3 large-up-4">
  {% for hero in site.heroes %}
    <div class="column column-block">
      <img src="{{ site.baseurl }}{{ hero.portrait }}" alt="{{ hero.title }}" class="thumbnail image--full">
      <h4><a href="{{ hero.url }}">{{ hero.title }}</a></h4>
    </div>
  {% endfor %}
</div>
