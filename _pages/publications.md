---
layout: page
permalink: /publications/
title: publications
workshop_years: [2020, 2019]
report_years: [2021]
nav: true
---

<center><h3><p style="color:#D41B2C">workshop papers</p></h3></center>

<div class="publications">
{% for y in page.workshop_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshop-papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

<center><h3><p style="color:#D41B2C">technical reports</p></h3></center>

<div class="publications">
{% for y in page.report_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f technical-reports -q @*[year={{y}}]* %}
{% endfor %}
</div>
