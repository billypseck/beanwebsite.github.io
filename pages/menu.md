---
title: Menu
layout: default
permalink: /menu/
---
<div class="flex-list flex-list-2-col">
{% for category in site.data.menu %}
<div class="menu-category flex-item ">

<h2 class="menu-item-category">{% if category.image %}
<img class="menu-item-category-image" src="{{ site.baseurl }}/assets/images/food/{{ category.image }}">
{% endif %}{{ category.category }}</h2>

<ul>
{% for item in category.items %}
<li class="menu-item">
<span class="menu-item-title">{{ item.title }}</span>
<span class="menu-item-price">${{ item.price }}</span>
<span class="menu-item-description">{{ item.shortDescription }}</span>
</li>
{% endfor %}
</ul>
</div>
{% endfor %}
</div>
