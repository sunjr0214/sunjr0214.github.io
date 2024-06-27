---
layout: page
permalink: /publications/
title: publications
description: This page only shows selected publications. The full publication list is available on <a href='https://scholar.google.com/citations?user=R2Y-OhQAAAAJ&hl=zh-CN'>google scholar</a>.
years: [2024, 2022, 2021, 2020, 2019, 2018, 2017, 2016]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
