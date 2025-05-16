---
layout: page
permalink: /publications/
title: Publications
description: 
nav: true
nav_order: 2

years: [2025, 2024, 2023, 2022]
sections:
    - title: Latest preprints
      filestem: preprints
    - title: Conference papers
      filestem: conferences
    - title: Journal papers
      filestem: journals
    - title: Workshop papers
      filestem: workshops
#    - title: Accepted to TACL
#     filestem: accepted_to_TACL
#    - title: PhD theses
#      filestem: dissertations
#    - title: Master's theses
#      filestem: theses
---
{% for sec in page.sections %}
<div class="publication-category">
    <h2>{{sec.title}}</h2>
    {% for y in page.years %}
        <!-- List for year {{y}}: -->
        {% bibliography -f {{sec.filestem}} -q @*[year={{y}}]* %}
    {% endfor %}
</div>
<hr>
{% endfor %}
