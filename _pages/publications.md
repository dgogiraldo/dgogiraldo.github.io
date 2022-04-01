---
layout: page
permalink: /publications/
title: referencias
description: Publicaciones destacadas referente al tema o que han servido de inspiración.
years: [1, 2, 3, 4]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
