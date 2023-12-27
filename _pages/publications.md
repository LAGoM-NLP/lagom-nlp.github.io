---
layout: page
permalink: /publications/
title: publications 
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016]
years_theses: [2019, 2014, 2013]
nav: true
---


<h1 class="category">Publications</h1>
<span id="publications"></span>


<div class="publications">

<!--
<h4 class="category">Preprints</h4>
{% for y in page.years %}
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}
</div>
-->

<br>
<div class="publications">
<h4 class="category"> Conference papers and journal articles</h4>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conf-papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

<br>
<div class="publications">
<h4 class="category"> Book chapters</h4>
{% for y in page.years %}
  {% bibliography -f book-chapters -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h4 class="category">Theses</h4>
{% for y in page.years_theses %}
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h4 class="category">Non-archival stuff</h4>
{% for y in page.years %}
  {% bibliography -f non-archival -q @*[year={{y}}]* %}
{% endfor %}
</div>