---
layout: about
title: Home
permalink: /
subtitle: 

description: >
    Welcome!
    We are the **Leuven AI Group on Multilingual NLP (LAGoM NLP)**, a research lab at the [Department of Computer Science](https://wms.cs.kuleuven.be/cs/english) at the University of Leuven (KU Leuven), directed by Prof. Dr. Miryam de Lhoneux.

profile:
  align: right
  image: logo/script-L_450px.png
  image_circular: false
  address: 

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page

groups: [members, affiliated]
members:
  title: Members
  people:
    - name: Miryam de Lhoneux
      description: Prof. Dr., Head of LAGoM NLP
      website: https://people.cs.kuleuven.be/~miryam.delhoneux/
      picture: https://media.licdn.com/dms/image/C4D03AQHPa7B6g4Ox3Q/profile-displayphoto-shrink_800_800/0/1549982999930?e=1709164800&v=beta&t=2CCKSDKBNkRWdmJNjWyc02FMJkwZPqHPtl7-yccPROo
    - name: Kushal J. Tatariya
      description: PhD student (2022–)
      website: 
      picture: https://media.licdn.com/dms/image/C4D03AQHawvM1ArUaIw/profile-displayphoto-shrink_800_800/0/1647871572663?e=1709164800&v=beta&t=L93kvzwuP2pQ9dcgTieC8LK6X1gJYd2ZZnFs-HDgIw8
    - name: Thomas Bauwens
      description: PhD student (2023–)
      website: https://bauwenst.github.io/
      picture: https://media.licdn.com/dms/image/D4D03AQEPzc_E1vJWLA/profile-displayphoto-shrink_800_800/0/1689027640596?e=1709164800&v=beta&t=IyBRnnVg0fg0M403BnxxCtRZp00kM1kVidvG_chCvkQ
    - name: Wessel Poelman
      description: PhD student (2023–)
      website: https://wesselpoelman.nl/
      picture: https://media.licdn.com/dms/image/D4E03AQFtGXi1irl-jQ/profile-displayphoto-shrink_800_800/0/1682423889310?e=1709164800&v=beta&t=K3L2ejprWwYfXFKRZSCRoO27sjG0juecLW6IIsnZEak
    - name: Artur Kulmizev
      description: Postdoc (2023–)
      website: https://akulmizev.com/
      picture: https://media.licdn.com/dms/image/C4D03AQG7nJOmd5_hug/profile-displayphoto-shrink_800_800/0/1549986124762?e=1709164800&v=beta&t=6OTo8MeyFuj7M7bikApnsiv1qVEi1OR-s00jhV8fbLI

affiliated:
  title: Affiliated members (e.g. co-supervisors, co-supervised or mentored external PhD students, guest researchers and visitors)
  people:
    - name: François Remy
      description: 
      website: https://fremycompany.com/
      picture: 
---

<!-- What follows will be put after the description box (see the about.html template). -->

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
              <img class="avatar" src="/assets/img/logo/script-L_450px.png" alt="Portrait ({{person.name}})" width="auto" height="auto">
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
  We are located at Celestijnenlaan 200A, 3001 Heverlee, Belgium.<br/>

  <a href="https://github.com/lagom-nlp"><i class="fab fa-github"></i> LAGoM on GitHub</a><br/>
  <a href="https://twitter.com/mdlhx"><i class="fab fa-twitter"></i> Miryam on X</a><br/>

</div>
