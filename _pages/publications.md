---
layout: page
permalink: /publications/
title: Publications
description: This section contains publications in which I was a primary analyzer or made significant contributions. I am an author on 559 papers by the CMS and ATLAS collaborations, as of 5 October 2023.
years: [2019, 2020, 2021, 2022, 2023]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">
{%- for y in page.years reversed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
<!-- <h5>Author on 437 papers by the CMS and ATLAS collaborations, as of 4 July 2022</h5> -->


