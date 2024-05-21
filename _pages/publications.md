---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
years: [2022, 2020, 2018, 2017, 2016, 2015]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
