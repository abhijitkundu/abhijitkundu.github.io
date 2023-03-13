---
layout: page
permalink: /publications/
title: publications
description: My research publications.
years: [2023, 2022, 2021, 2020, 2018, 2017, 2016, 2015, 2014, 2012, 2011, 2010, 2009]
nav: true
---
Also see my [google scholar](https://scholar.google.com/citations?user=GGcjtCsAAAAJ&h) <i class="ai ai-google-scholar ai-1x"></i> page.
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
