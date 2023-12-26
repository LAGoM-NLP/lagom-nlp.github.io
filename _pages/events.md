---
layout: page
permalink: /events/
title: Events
description: 
nav: true
nav_order: 5
---
<div class="events">
    <!-- events are sorted by filename (reverse order) -->
    {%- for e in site.events reversed -%}
        <div class="event">
	        {% include event.html event=e %}
        </div>
    {%- endfor %}
</div>