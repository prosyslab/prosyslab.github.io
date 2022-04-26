---
title: "Photos"
layout: piclay
permalink: /photos.html
---

## Photos

<div class="list-group">
{%- for photo in site.data.photos -%}
<a href="{{ photo.link }}" class="list-group-item list-group-item-action">{{ photo.title }}<span class="badge badge-primary badge-pill">{{ photo.date }}</span></a>
{% endfor %}
</div>
