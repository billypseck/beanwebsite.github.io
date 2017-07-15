---
layout: default
title: Coffee
permalink: /coffee/
---

<ul class="coffee-list flex-list flex-list-3-col">
{% assign sorted = (site.coffee | sort: 'sortOrder') %}
 {% for coffee in sorted %}
  <li class="coffee-list-item flex-item">
    <div class="flex-item-content">
    <a href="{{ coffee.title | slugify }}/">
      <img src="{{site.baseurl}}{{ coffee.smallImage }}"/>
      <span class="coffee-name">{{ coffee.title }}</span>
    </a>
    <p class="coffee-description">{{ coffee.shortDescription }}</p>
    </div>
  </li>
{% endfor %}
</ul>
