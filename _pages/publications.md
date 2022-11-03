---
layout: page
permalink: /publications/
title: publications
description: Peer-reviewed papers published during my time as a PhD student. I was working on new efficient methods to simulate the (quantum) dynamics of chemical reactions.
years: [2022, 2021, 2020]
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
