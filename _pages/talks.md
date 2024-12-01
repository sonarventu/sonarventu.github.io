---
layout: page
permalink: /talks/
title: talks
description: Past and upcoming talks and seminars.
years: [2024, 2023, 2022]
nav: true
nav_order: 3
---

<div class="talks">

{%- for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  <ul>
    {% bibliography -f talks -q @*[year={{ y }}]* %}
  </ul>
{%- endfor %}

</div>