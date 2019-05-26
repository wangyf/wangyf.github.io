---
title: "Steve's Gallery"
layout: piclay
excerpt: "Steve's Gallery"
permalink: /stevegallery/
---

# Gallery
(Right-click *'view image'* or *'open image in new tab'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.steveday %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/symposium/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
<i>{{ pic.info }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}


