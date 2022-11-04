---
layout: page
permalink: /publications/
title: Publications
description: Selected Publications by categories in reversed chronological order. Please refer to my [Google Scholar](https://scholar.google.com/citations?user=citations?user=k4SdlbcAAAAJ&hl=en&user=k4SdlbcAAAAJ) for the full list.
years: [2022,2021,2020,2019,2018,2017,2016]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
