---
layout: basic
permalink: "/testimonials/"
title: Testimonials
status: published
# imgBanner: /assets/images/pages/
# imgThumbnail: /assets/images/pages/
---

{% for testimony in site.testimonials %}
<div class="row">
<div class="large-3 columns">
<img src="{{ site.baseurl }}{{ testimony.portrait }}" alt="{{ testimony.title }}" class="thumbnail image--full">
</div>
<div class="large-9 columns">
<h4>{{ testimony.title }}</h4>
{{ testimony.content }}
</div>
</div>
<hr>
{% endfor %}
