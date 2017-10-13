---
layout: basic
permalink: "/our-partners/"
title: Our partners
status: published
# imgBanner: /assets/images/pages/
# imgThumbnail: /assets/images/pages/
---

{% for partner in site.partners %}
<div class="row">
<div class="large-3 columns">
<img src="{{ site.baseurl }}{{ partner.portrait }}" alt="{{ partner.title }}" class="thumbnail image--full">
</div>
<div class="large-9 columns">
<h4>{{ partner.title }}</h4>
{{ partner.content }}
</div>
</div>
<hr>
{% endfor %}
