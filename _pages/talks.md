---
layout: default
permalink: /talks/
title: talks
description: past and upcoming talks and seminars.
nav: true
nav_order: 3
---

<div class="post">
  <header class="post-header">
    <h1 class="post-title">{{ page.title }}</h1>
  </header>
  <article>
    <ul>
      {% for talk in site.data.talks %}
        <li>
          <strong>{{ talk.title }}</strong>
          {% if talk.slides and talk.slides != "" %}
            - <a href="{{ talk.slides }}" target="_blank">Slides</a>
          {% else %}
            - *(No slides available)*
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  </article>
</div>