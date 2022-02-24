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
  <p> [{{ publi.news3 }}]({{publi.news3link}})</p>
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
  {{ publi.authors }} (<em>{{ publi.year }}</em>), {{ publi.title }}, <em>{{publi.journal}}</em>, {{publi.volume}}, <a href="https://doi.org/{{ publi.doi }}">doi:{{ publi.doi }}</a>  [<strong>PDF</strong>]({{ site.baseurl }}/pdf/{{publi.pdf}})
{% endif %}
{% if publi.cat == "submitted"%}
  {{ publi.authors }} (<em>{{ publi.year }}</em>), {{ publi.title }}, <em>{{publi.journal}}</em>, {{publi.volume}}
{% endif %}
{% endfor %}

<br>

#### Non Peer-review publication
------------------
{% for publi in site.data.publist %}
{% if publi.cat == "nonjournal"%}
  {{ publi.authors }} (<em>{{ publi.year }}</em>), {{ publi.title }} <em>{{publi.journal}}</em>, {{publi.volume}}, <a href="{{publi.link.url}}">{{ publi.link.url }}</a> [<strong>PDF</strong>]({{ site.baseurl }}/pdf/{{publi.pdf}}) 
{% endif %}
{% endfor %}



-----------------------------
#### Leave me a message
<html>
<form id="fs-frm" name="simple-contact-form" accept-charset="utf-8" action="https://formspree.io/f/xwkyozkl" method="post">
  <fieldset id="fs-frm-inputs">
    <label for="full-name">Full Name</label>
    <input type="text" name="name" id="full-name" placeholder="First and Last" required="">
    <label for="email-address">Email Address</label>
    <input type="email" name="_replyto" id="email-address" placeholder="email@domain.tld" required="">
    <label for="message">Message</label>
    <textarea rows="5" name="message" id="message" placeholder="Aenean lacinia bibendum nulla sed consectetur. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Donec ullamcorper nulla non metus auctor fringilla nullam quis risus." required=""></textarea>
    <input type="hidden" name="_subject" id="email-subject" value="Contact Form Submission">
  </fieldset>
  <input type="submit" value="Submit">
</form><style>/* reset */
#fs-frm input,
#fs-frm select,
#fs-frm textarea,
#fs-frm fieldset,
#fs-frm optgroup,
#fs-frm label,
#fs-frm #card-element:disabled {
  font-family: inherit;
  font-size: 100%;
  color: inherit;
  border: none;
  border-radius: 0;
  display: block;
  width: 100%;
  padding: 0;
  margin: 0;
  -webkit-appearance: none;
  -moz-appearance: none;
}
#fs-frm label,
#fs-frm legend,
#fs-frm ::placeholder {
  font-size: 1.925rem;
  margin-bottom: 0.9rem;
  padding-top: .2rem;
  display: flex;
  align-items: baseline;
}

/* border, padding, margin, width */
#fs-frm input,
#fs-frm select,
#fs-frm textarea,
#fs-frm #card-element {
  border: 4px solid rgba(153, 27, 30,0.6);
  background-color: rgba(255, 199, 44,0.6);
  padding: .75em 1rem;
  margin-bottom: 1.5rem;
}
#fs-frm input:focus,
#fs-frm select:focus,
#fs-frm textarea:focus {
  background-color: white;
  outline-style: solid;
  outline-width: thin;
  outline-color: gray;
  outline-offset: -1px;
}
#fs-frm [type="text"],
#fs-frm [type="email"] {
  width: 100%;
}
#fs-frm [type="button"],
#fs-frm [type="submit"],
#fs-frm [type="reset"] {
  width: auto;
  cursor: pointer;
  -webkit-appearance: button;
  -moz-appearance: button;
  appearance: button;
}
#fs-frm [type="button"]:focus,
#fs-frm [type="submit"]:focus,
#fs-frm [type="reset"]:focus {
  outline: none;
}
#fs-frm [type="submit"],
#fs-frm [type="reset"] {
  margin-bottom: 0;
}
#fs-frm select {
  text-transform: none;
}

#fs-frm [type="checkbox"] {
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  appearance: checkbox;
  display: inline-block;
  width: auto;
  margin: 0 .5em 0 0 !important;
}

#fs-frm [type="radio"] {
  -webkit-appearance: radio;
  -moz-appearance: radio;
  appearance: radio;
}

/* address, locale */
#fs-frm fieldset.locale input[name="city"],
#fs-frm fieldset.locale select[name="state"],
#fs-frm fieldset.locale input[name="postal-code"] {
  display: inline;
}
#fs-frm fieldset.locale input[name="city"] {
  width: 52%;
}
#fs-frm fieldset.locale select[name="state"],
#fs-frm fieldset.locale input[name="postal-code"] {
  width: 20%;
}
#fs-frm fieldset.locale input[name="city"],
#fs-frm fieldset.locale select[name="state"] {
  margin-right: 3%;
}
</style>

</html>
<br/>
<br/>
<br/>