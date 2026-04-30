---
layout: page
permalink: /publications/
title: publications
description: 
years: [2026,2024,2023,2021]
nav: true
---

<div class="publications">

<p><small>* = co-first author, # = corresponding author</small></p>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
