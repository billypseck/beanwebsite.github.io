---
title: Menu
layout: default
permalink: /menu/
---

{% for category in site.data.menu %}
<h2>{{ category.category }}</h2>
<ul>
{% for item in category.items %}
<li>
{{ item.title }}<br>
{{ item.price }}<br>
{{ item.shortDescription }}
</li>
{% endfor %}
</ul>
{% endfor %}
