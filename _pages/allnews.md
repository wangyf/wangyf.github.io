---
title: "News"
layout: textlay
excerpt: "Yongfei Wang"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
{{article.date }} <br>
<strong>{{ article.headline }} </strong>

{% endfor %}

