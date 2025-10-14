---
layout: page
permalink: /talks/
title: talks
description: Here's a list of my talks and seminars.
years: [2025,2024, 2023, 2022]
nav: true
nav_order: 3
---

<div class="publications">

{%- for y in page.years %}
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>