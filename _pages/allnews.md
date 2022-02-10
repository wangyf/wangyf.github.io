---
title: "News"
layout: textlay
excerpt: "Yongfei Wang"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<h3>{{article.date }} </h3> 
<h4>{{article.headline |replace:'max-width: 192px','max-width: 930px' }}</h4> <br>

{% endfor %}

