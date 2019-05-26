---
title: "Yongfei Wang - Publications"
layout: gridlay
excerpt: "Yongfei Wang -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Highlights

(For a full list see [below](#full-list) or go to [ResearcherGate](https://www.researchgate.net/profile/Yongfei_Wang3))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-15 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" style="width: 400px; height: 250px; float: left; border: 20px" />
  <p></p>
  <p>{{ publi.description }}</p>
  <p>{{ publi.authors }}</p>
  <em>{{publi.journal}}</em> (<em>{{ publi.year }}</em>) 
  <p><em><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></em> [<strong>PDF</strong>]({{ site.baseurl }}/pdf/{{publi.pdf}}) </p>
  <p> </p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> [{{ publi.news2 }}]({{publi.news2link}})</p>
  <p> 1. {{publi.key1}}</p>
  <p> 2. {{publi.key2}}</p>
  <p> 3. {{publi.key3}}</p>
  <p> <br><br></p>

 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


# Full List

#### Peer-review Journal publication
------------------
{% for publi in site.data.publist %}
{% if publi.cat == "journal"%}
  {{ publi.authors }} (<em>{{ publi.year }}</em>) <em>{{publi.journal}}</em>, {{publi.volume}}, <a href="https://doi.org/{{ publi.doi }}">doi:{{ publi.doi }}</a> 
{% endif %}
{% endfor %}

<br>

#### Non Peer-review publication
------------------
{% for publi in site.data.publist %}
{% if publi.cat == "nonjournal"%}
  {{ publi.authors }} (<em>{{ publi.year }}</em>) <em>{{publi.journal}}</em>, {{publi.volume}}, <a href="https://doi.org/{{ publi.doi }}">doi:{{ publi.doi }}</a> 
{% endif %}
{% endfor %}

