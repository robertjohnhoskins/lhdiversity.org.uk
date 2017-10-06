---
layout: basic
permalink: "/our-team/"
section: /our-team
title: Our team
status: published
# imgBanner: /assets/images/pages/
# imgThumbnail: /assets/images/pages/
---

<div class="row small-up-2 medium-up-3 large-up-4">
  {% for member in site.team %}
    {% if member.layout == "team-member" %}
      <div class="column column-block">
        <img src="{{ site.baseurl }}{{ member.portrait }}" class="thumbnail image--full" alt="{{ member.title }}">
        <h4><a href="{{ member.url | prepend: site.baseurl }}">{{ member.title }}</a></h4>
        <h5>{{ member.position }}</h5>
      </div>
    {% endif %}
  {% endfor %}
</div>
