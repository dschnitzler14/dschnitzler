---
title:
layout: default
permalink: #/research_projects/
published: true
---

<div class="ProjectContainer">

    <div class="gallery">

{% for research_project in site.research_projects %}

{% if research_project.redirect %}

  <div class="projectTile">
          <a href="{{ research_project.redirect }}" target="_blank">
          <span>
              <h2>{{research_project.tag }} {{ research_project.title }}</h2>
              <br/>
              <p>{{ research_project.description }}</p>
          </span>
          </a>
  </div>

{% else %}

  <div class="projectTile">
          <a href="{{ research_project.url | prepend: site.url }}">
          <span>
              <h2>{{research_project.tag }} {{ research_project.title }}</h2>
              <br/>
              <p>{{ research_project.description }}</p>
          </span>
          </a>
  </div>

{% endif %}

{% endfor %}

    </div>

</div>
