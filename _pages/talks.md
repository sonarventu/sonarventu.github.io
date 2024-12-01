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

<!-- 
# This is the old content of this file. It relied on the file data/talks.yml. However this approach doesn't work, and I'm tired of troubleshooting.
---
layout: default
permalink: /talks/
title: talks
description: Past and upcoming talks and seminars.
nav: true
nav_order: 3
---

#<p>&nbsp;</p> Coming soon...

<div class="post">
  <header class="post-header">
    <h1 class="post-title">{{ page.title }}</h1>
  </header>
  <article>
    <ul>
      {% t %}
      <li>
        <strong>{{ talk.title }}</strong> <br>
        {{ talk.event }} — {{ talk.date }} <br>
        {{ talk.location }}
        {% if talk.slides and talk.slides != "" %}
        (<a href="{{ talk.slides }}" target="_blank">Slides</a>)
        {% endif %}
      </li>
      {% endfor %}
    </ul>
  </article>
</div> -->