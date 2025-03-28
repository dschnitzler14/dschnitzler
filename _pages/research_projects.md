---
title:
layout: default
permalink: /research_projects/
published: true
---

<div class="ProjectContainer">

    <div class="gallery">

{% for research_project in site.research_projects %}

  <div class="projectTile">
      {% if research_project.dg_link %}
          <a href="{{ research_project.dg_link }}" target="_blank">
      {% elsif research_project.redirect %}
          <a href="{{ research_project.redirect }}" target="_blank">
      {% else %}
          <a href="{{ research_project.url | prepend: site.baseurl | prepend: site.url }}">
      {% endif %}
          <span>
              <h2>{{ research_project.tag }} {{ research_project.title }}</h2>
              <br/>
              <p>{{ research_project.description }}</p>
          </span>
          </a>
  </div>

{% endfor %}

    </div>

</div>
