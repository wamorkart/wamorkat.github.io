---
layout: page
permalink: /publications/
title: Publications
description: Publications and Presentations
years: [2019, 2021, 2022]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
<h5>Author on 437 papers by the CMS and ATLAS collaborations, as of 4 July 2022</h5>
