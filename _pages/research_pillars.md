---
title:
layout: default
permalink: /research_pillars/
published: true
---
<h2 class="post-headline">Science</h2>

<div class="ProjectContainer">

  <div class="gallery">

    {% for research_pillar in site.research_pillars %}
      <div class="pillarTile">
        <a href="{{ research_pillar.url | relative_url }}">
          <span>
            <h2>{{ research_pillar.title }}</h2>
            <br/>
            <p>{{ research_pillar.description }}</p>
          </span>
        </a>
      </div>
    {% endfor %}

  </div>

</div>
