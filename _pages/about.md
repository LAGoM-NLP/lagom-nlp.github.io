---
layout: about
title: Home
permalink: /
subtitle: 

profile:
  align: right
  image: script-L.png
  image_circular: false
  address: 

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page

groups: [members, affiliated]
members:
  title: Members
  people:

affiliated:
  title: Affiliated members (e.g. co-supervisors, co-supervised or mentored external PhD students, guest researchers and visitors)
  people:
---

Welcome!

<div id="main-body" class="projects">
  <h2 class="category">News</h2>
  <ul>
    <li>No news yet. Stay tuned!</li>
  </ul>

  <h2 class="category">Events</h2>
  <ul>
    <li>No events yet. Stay tuned!</li>
  </ul>

  {%- for group in page.groups -%}
  <h2 class="category">{{page.[group].title}}</h2>
    <div class="grid">
      {%- for person in page.[group].people -%}
          <article class="grid-item card">
            {% if person.picture -%}
              <img class="avatar" src="/assets/img/{{person.picture}}" alt="Portrait ({{person.name}})" width="auto" height="auto">
            {%- else -%}
              <img class="avatar" src="/assets/img/script-L.png" alt="Portrait ({{person.name}})" width="auto" height="auto">
            {%- endif -%}
          <div class="card-body">
            <!-- <h2 class="card-title">{{person.name}}</h2> -->
            <h2 class="card-title">
              {% if person.website -%}
                <a href="{{person.website}}">{{person.name}}</a>
              {%- else -%}
                {{person.name}}
              {%- endif -%}
            </h2>
            <div class="card-text">
              {{person.description}}
              <!-- <p style="margin-bottom: 0rem;">{{person.description}}</p> 
              <ul class="network-icon" aria-hidden="true">
              {% if person.website -%}
                <li><a href="{{person.website}}"><i class="fas fa-globe"></i></a></li>
              {%- endif -%}
              {% if person.email -%}
                <li><a role="button" class="email" style="color: var(--global-theme-color)"><i class="fas fa-envelope"></i></a></li>
              {%- endif -%}
              {% if person.googlescholar -%}
                <li><a href="{{person.googlescholar}}"><i class="ai ai-google-scholar"></i></a></li>
              {%- endif -%}
              {% if person.github -%}
                <li><a href="{{person.github}}"><i class="fab fa-github"></i></a></li>
              {%- endif -%}
              {% if person.twitter -%}
                <li><a href="{{person.twitter}}"><i class="fab fa-twitter"></i></a></li>
              {%- endif -%}
            </ul>
            {% if person.email -%}
              <div class="email hidden">
                <p>{{ person.email }}</p>
              </div>
            {%- endif -%} -->
              </div>
            </div>
          </article>
      {%- endfor -%}
    </div>
  {%- endfor -%}

<!--
  <h2 class="category">Funding</h2>
  Our research is supported by:
  <ul>
    <li><a href="https://erc.europa.eu/homepage">European Research Council (ERC)</a> project <a href="https://mainlp.github.io/projects/#ongoingproj">DIALECT</a></li>
    <li><a href="https://dff.dk/en">Danmarks Frie Forskningsfond (DFF)</a>, Sapere Aude Research Leader grant</li>
    <li><a href="https://www.bayern.de/politik/hightech-agenda/">Bayerische Staatsregierung HTA</a></li>
    <li><a href="https://mcml.ai/">Munich Center for Machine Learning (MCML)</a></li>
    <li><a href="https://www.bidt.digital/">Bayerisches Forschungsinstitut für Digitale Transformation (bidt)</a></li>
  </ul>
-->  
  <h2 class="category">Find us</h2>
  Somewhere in the world.

</div>
