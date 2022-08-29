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

### PhD Students
{% for member in site.data.members.phd %}
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

### Master Students
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

### Alumni

<table style="border-bottom:0px">
{% for member in site.data.members.alumni %}
  <tr style="border-bottom:0px">
    <td width="75%" style="border-bottom:0px">
      <h3 style="margin-top:0px">{{ member.name }} ({{ member.name-korean }})</h3>
      <i>{{ member.info }}, {{ member.year }}, {{ member.occupation }}.</i>
      <a href="{{ member.homepage }}"><i class="fas fa-home" style="color:#1B4F72"></i></a>
      <a href="mailto:{{ member.email }}"><i class="fas fa-envelope" style="color:#1B4F72"></i></a>
    </td>
  </tr>
{% endfor %}
</table>
