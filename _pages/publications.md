---
layout: page
permalink: /publications/
order: 4
title: publications
description: 
years: [2023, 2022, 2021, 2020, 2018]
nav: true
---

Please see the [Google Schloar](https://scholar.google.com/citations?hl=en&user=Ro9JqbEAAAAJ&view_op=list_works&sortby=pubdate) page for the most recent updates.

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
