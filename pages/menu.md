---
title: Menu
layout: default
permalink: /menu/
page_header_image: /assets/images/coverphotos/veg-bagle-delux.jpg
# page_header_image: /assets/images/coverphotos/mediteranian.jpg

---
<div class="flex-list flex-list-2-col">
{% for category in site.data.menu %}
<div class="menu-category flex-item ">
<div class="flex-item-content">
<h2 class="menu-item-category">
  {{ category.category }}
</h2>
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
</div>
{% endfor %}
</div>
