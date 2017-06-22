---
layout: default
title: Coffee
permalink: /coffee/
---
<ul class="coffee-list flex-list flex-list-4-col">
{% assign sorted = (site.coffee | sort: 'sortOrder') %}
 {% for coffee in sorted %}
  <li class="coffee-list-item">
    <a href="{{ coffee.title | slugify }}/">
      <img src="{{ coffee.smallImage }}"/>
      <span class="coffee-name">{{ coffee.title }}</span>
    </a>
    <p class="coffee-description">{{ coffee.shortDescription }}</p>
  </li>
{% endfor %}
</ul>
