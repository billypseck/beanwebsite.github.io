---
title: Menu
layout: default
permalink: /menu/
---

{% for category in site.data.menu %}
<div class="menu-category">
<h2 class="menu-item-category">{{ category.category }}</h2>
<ul>
{% for item in category.items %}
<li class="menu-item">
<span class="menu-item-title">{{ item.title }}</span>. . . . . . . .
<span class="menu-item-price">{{ item.price }}</span>
<span class="menu-item-description">{{ item.shortDescription }}</span>
</li>
{% endfor %}
</ul>
</div>
{% endfor %}
