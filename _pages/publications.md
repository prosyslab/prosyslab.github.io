---
title: "Prosys Lab - Publications"
layout: gridlay
excerpt: "Prosys Lab -- Publications."
sitemap: false
permalink: /publications/
---

## Publications
<!--
## Group highlights

(For a full list of publications and patents see [below](#full-list-of-publications) or go to [Google Scholar](https://scholar.google.ch/citations?user=TqxYWZsAAAAJ), [ResearcherID](https://www.researcherid.com/rid/D-7763-2012))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
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
-->

{% assign year_printed = 0 %}
{% assign list_opened = false %}

{% for pub in site.data.publications %}
{% if year_printed != pub.year %}
{% if list_opened == true %}
</ul>
{% endif %}
<h3> {{ pub.year }} </h3>
<ul>
{% assign list_opened = true %}
{% assign year_printed = pub.year %}
{% endif %}
<li>{{pub.title}}<br>
{% for author in pub.author %}
{% if forloop.last %}
and {{ author }}
{% else %}
{{ author }},
{% endif %}
{% endfor %}
  {% if pub.award != nil %}
    <br>&#127942; <b>{{pub.award}}</b>
  {% endif %}
  {% if pub.misc != nil %}
  <br><b>{{ pub.misc }}</b>
  {% endif %}
  <br>
  <a href="{{ pub.venue_link }}">{{ pub.venue }}</a>, {{ pub.year }}
   <br>
  {% if pub.paper != nil %}
  [<a href="{{ site.baseurl }}/publications/{{ pub.paper }}">paper</a>]
  {% endif %}
  {% if pub.full != nil %}
    [<a href="{{ site.baseurl }}/publications/{{ pub.full }}">full-version</a>]
  {% endif %}
  {% if pub.slides != nil %}
    [<a href="slides/{{ pub.slides }}">slides</a>]
  {% endif %}
  {% if pub.video != nil %}
    [<a href="{{ pub.video }}">video</a>]
  {% endif %}
  {% if pub.code != nil %}
    [<a href="{{ pub.code }}">code</a>]
  {% endif %}
  </li>
  <br>
{% endfor %}
