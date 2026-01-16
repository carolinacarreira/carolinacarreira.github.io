---
layout: page
permalink: /_publications/
title: _publications
description: publications by categories in reversed chronological order. 
years: [2022, 2021, 1905]
nav: true
published: false
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
