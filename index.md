---
layout: about
permalink: /
profile:
  align: right
  image: profile.jpg
published: true
---
<p class="currently-reading">
  {% assign currently_reading = site.bookshelf | where: "status", "📖" | limit: 1 %}
  {% if currently_reading.size > 0 %}
    Currently Reading: 
    {% if currently_reading[0].book_link %}
      <a href="{{ currently_reading[0].book_link }}" target="_blank"><strong>{{ currently_reading[0].book_title }}</strong></a>
    {% else %}
      <strong>{{ currently_reading[0].book_title }}</strong>
    {% endif %}
    by {{ currently_reading[0].book_author }}
  {% else %}
    Not currently reading any books.
  {% endif %}
</p>

I am a postdoctoral researcher with a PhD in neuroscience who thrives on learning and discovery. My work spans neuroscience, with a focus on neuroendocrinology and affective disorders, alongside education research and meta-science. I develop open research and teaching tools, and critically examine how emerging technologies such as generative AI are shaping scholarship. I am also the founder of Paperstars, a community-driven platform for post-publication rating, with to goal to help uncouple science from publication metrics. I am passionate about the academic environment, where I continuously expand my knowledge while sharing it with others, and my ability to communicate complex concepts in a clear and engaging way has made me an effective and enthusiastic educator. I am fully bilingual in English and German, and proficient in French.


<div class="work-table">
  <div class="work-row">
    <span class="work-type">Research</span>
    <div>
      <p class="work-title">Evolutionary Origins of Depression</p>
      <p class="work-desc">Examining a framework proposing depression as a dysregulated energy conservation mechanism, analogous to mammalian hibernation.</p>
      <a class="work-link" href="/_research_pillars/02_depression">Read more</a>
    </div>
  </div>
  <div class="work-row">
    <span class="work-type">Platform</span>
    <div>
      <p class="work-title">Paperstars</p>
      <p class="work-desc">Uncoupling science from publication metrics. Goodreads, but for Science.</p>
      <a class="work-link" href="https://paperstars.org">Read more</a>
    </div>
  </div>
  <div class="work-row">
    <span class="work-type">Educational</span>
    <div>
      <p class="work-title">Scientific Literacy Tools</p>
      <p class="work-desc">Open-source tools for teaching scientific literacy.</p>
      <a class="work-link" href="/_research_pillars/01_education">Read more</a>
    </div>
  </div>
  <div class="work-row">
    <span class="work-type">Metascience</span>
    <div>
      <p class="work-title"> Thinking about the <i>status quo</i></p>
      <p class="work-desc">Various writing and presentations on scientific culture</p>
      <a class="work-link" href="/_research_pillars/03_meta-science">Read more</a>
    </div>
  </div>
</div>
