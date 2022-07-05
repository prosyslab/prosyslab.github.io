---
layout: single
title: "Members"
permalink: /members/
author_profile: false
---

### Professor

{% for member in site.data.members.professor %}
<table style="border-bottom:0px !important;">
  <tr style="border-bottom:0px !important;">
    <td width="25%" style="border-bottom:0px !important;">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/images/members/{{ member.photo }}" />
    </td>
    <td width="75%" style="border-bottom:0px !important;">
      <h3>{{ member.name }} ({{ member.name-korean }})</h3>
      <i>Assistant Professor</i>
      <a href="{{ member.homepage }}"><i class="fas fa-home" style="color:#1B4F72"></i></a>
      <a href="mailto:{{ member.email }}"><i class="fas fa-envelope" style="color:#1B4F72"></i></a>
      <br><br>
    </td>
  </tr>
</table>
{% endfor %}

### Students
{% for member in site.data.members.master %}
<table style="border-bottom:0px !important;">
  <tr style="border-bottom:0px !important;">
    <td width="25%" style="border-bottom:0px !important;">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/images/members/{{ member.photo }}" />
    </td>
    <td width="75%" style="border-bottom:0px !important;">
      <h3>{{ member.name }} ({{ member.name-korean }})</h3>
      <i>{{ member.info }}</i>
      <a href="{{ member.homepage }}"><i class="fas fa-home" style="color:#1B4F72"></i></a>
      <a href="mailto:{{ member.email }}"><i class="fas fa-envelope" style="color:#1B4F72"></i></a>
      <br><br>
    </td>
  </tr>
</table>
{% endfor %}

<!--
## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
-->
<!--
## Former visitors, BSc/ MSc students
<div class="row">

<div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitors %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Master students</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
{% endfor %}
</div>
</div>
-->
