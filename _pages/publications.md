---
layout: page
permalink: /publications/
title: publications
description: <h5>You can find my publications below or on my <a href = 'https://scholar.google.com/citations?authuser=1&user=bGcmLqYAAAAJ'>Google Scholar page</a>.</h5>
years: [2026,2025,2023,2022,2019]
nav: true
nav_order: 1

---

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
