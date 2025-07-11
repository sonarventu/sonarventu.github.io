---
layout: page
permalink: /publications/
title: publications
description: Here are my publications, year by year, in reversed chronological order.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<style>
.publications {
  counter-reset: pub-number;
}

.publications li::before {
  counter-increment: pub-number;
  content: counter(pub-number) ". ";
  display: inline-block;
  margin-right: 0.5em;
}
</style>

<div class="publications">
  {% bibliography --sort_by year --order ascending %}
</div>