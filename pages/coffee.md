---
layout: default
title: Coffee
permalink: /coffee/
---
<ul class="projects flex-list flex-list-4-col">
{% assign sorted = (site.coffee | sort: 'sortOrder') %}
 {% for coffee in sorted %}
  <li class="project-item">
    <a href="{{ coffee.title | slugify }}/" class="project-name">
      <img src="{{ coffee.smallImage }}"/>
      {{ coffee.title }}
    </a>
    <p>{{ coffee.shortDescription }}</p>
  </li>
{% endfor %}
</ul>
