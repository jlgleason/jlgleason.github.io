---
layout: page
permalink: /publications/
title: publications
before_neu_years: [2021, 2020, 2019]
neu_years: [2025, 2024, 2023]
nav: true
nav_order: 2
---

<!-- <center><h1><p style="color:#D41B2C">Northeastern</p></h1></center> -->

<div class="publications">
{% for y in page.neu_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f neu -q @*[year={{y}}]* %}
{% endfor %}
</div>

<!-- <center><h1><p style="color:#D41B2C">Before Northeastern</p></h1></center> -->

<div class="publications">
{% for y in page.before_neu_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f before-neu -q @*[year={{y}}]* %}
{% endfor %}
</div>
