---
layout: page
permalink: /publications/
title: Publications
description: 
nav: true
nav_order: 2

years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016]
sections:
    - title: Latest preprints
      filestem: preprints
    - title: Conference papers
      filestem: conferences
    - title: Journal articles
      filestem: journals
    - title: Workshop submissions
      filestem: workshops
    - title: PhD theses
      filestem: dissertations
    - title: Master's theses
      filestem: theses
---
{% for sec in page.sections %}
<br>
<div class="publications">
<h2>{{sec.title}}</h2>
{% for y in page.years %}
    {% bibliography -f {{sec.filestem}} -q @*[year={{y}}]* %}
{% endfor %}
</div>
{% endfor %}
