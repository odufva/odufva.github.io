---
layout: page
permalink: /publications/
title: publications
description:
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
selected_papers: true
nav: true
---

<div class="publications">
  <h2>selected publications</h2>
  {% bibliography -f papers -q @*[selected=true]* %}
</div>



<div class="publications">
<h2>all publications</h2>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
