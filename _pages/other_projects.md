---
title:
layout: default
permalink: /other_projects/
published: true
---

<div class="ProjectContainer">

    <div class="gallery">

  {% for other_project in site.other_projects %}

  {% if other_project.redirect %}

  <div class="projectTile">
          <a href="{{ other_project.redirect }}" target="_blank">
          <span>
              <h2>{{other_project.tag }} {{ other_project.title }}</h2>
              <br/>
              <p>{{ other_project.description }}</p>
          </span>
          </a>
  </div>

{% else %}

  <div class="projectTile">
          <a href="{{ other_project.url | prepend: site.baseurl | prepend: site.url }}">
          <span>
              <h2>{{other_project.tag }} {{ other_project.title }}</h2>
              <br/>
              <p>{{ other_project.description }}</p>
          </span>
          </a>
  </div>

{% endif %}

{% endfor %}

  </div>

</div>
