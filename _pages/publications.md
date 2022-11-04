---
layout: page
permalink: /publications/
title: Publications
description: Selected Publications by categories in reversed chronological order. Please refer to my <a href="https://scholar.google.com/citations?hl=zh-CN&user=k4SdlbcAAAAJ">[Google Scholar]</a> for the full list.
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
