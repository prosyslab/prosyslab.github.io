---
layout: default
title: People
image: /img/lab.jpg
---

<div class="content">
  <h2>Professor</h2>
  {% for prof in site.data.people.professor %}
  <p class="subtitle is-5">{{ prof.name }} ({{ prof.name-korean }})
     <a href="{{ prof.homepage }}"><i class="fas fa-home" style="color:#1B4F72"></i></a>
     <a href="mailto:{{ prof.email }}"><i class="fas fa-envelope" style="color:#1B4F72"></i></a>
  </p>
  {% endfor %}
  <br>
  <h2>Students</h2>
  {% for ms in site.data.people.master %}
    <p class="subtitle is-5">{{ ms.name }} ({{ ms.name-korean }})
    <a href="{{ ms.homepage }}"><i class="fas fa-home" style="color:#1B4F72"></i></a>
    <a href="mailto:{{ ms.email }}"><i class="fas fa-envelope" style="color:#1B4F72"></i></a>
  </p>
  {% endfor %}
  {% for ms in site.data.people.undergrad %}
    <p class="subtitle is-5">{{ ms.name }} ({{ ms.name-korean }})
      <a href="{{ ms.homepage }}"><i class="fas fa-home" style="color:#1B4F72"></i></a>
      <a href="mailto:{{ ms.email }}"><i class="fas fa-envelope" style="color:#1B4F72"></i></a>
    </p>
  {% endfor %}
</div>
