---
layout: about
permalink: /
profile:
  align: right
  image: profile.png
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

# Hey there! I'm Danny,

a post-doctoral researcher who loves blending science, coding, and creativity. I finished my PhD at the University of Edinburgh and now, I’m diving into new research at the Medical School Berlin with [Melanie Stefan](https://melaniestefan.net/){:target="\_blank"}. I’m all about learning and growing, and sharing my journey along the way.

I grew up in Vienna, Austria, but thanks to my American mum, I’ve always been fluent in English and German. In 2011, I made the leap to Scotland to study Biomedical Science at Aberdeen University. After graduating with my honours degree and integrated masters (MSci), I moved to Edinburgh to kick off my PhD, focusing on anxiety using a prenatal stress rat model. Through the course of my PhD I surprised myself and everyone around me when I really fell in love with coding.

<div class="bottomLinkTile">
  <a href="{{ '/research_projects/00_PhD_reflections' | relative_url }}">
    <i class="fa-solid fa-pen-nib"></i> Read my Reflections on my PhD
  </a>
</div>

<hr />

## Right now, I’m:

Focussing on my passions:

1. Passionate about making science open and accessible, working on projects aimed at fixing some of the problems in scientific publishing. I am also increasingly concerned about the use of GenAI in academia and am working on looking at that too. ([more on that here](/_research_pillars/03_meta-science))
2. Running Paperstars - a platfrom where researchers can anonymously rate and review paper, like Goodreads, but for science! [Check it out here](https://paperstars.org/){:target="\_blank"}
3. Looking at depression through an evolutionary lens ([read more here](/_research_pillars/02_depression))
4. Involved in a number of educational projects ([check it out here](/_research_pillars/01_education))

When I’m not deep in research, I love teaching and sharing knowledge. I'm contributing to the design of a course on the scientific process at the Medical School, as well as contributing to teaching and course design, and I’ve developed a cool interactive Shiny app for students to learn the fundamentals of scientific research ([more details here](/research_projects/01_blinkr)). I also get to co-supervise one of our amazing PhD students!

<div class="bottomLinkTile">
  <a href="{{ '/research_pillars' | relative_url }}">
    Go to Research Projects Page.
  </a>
</div>

<hr />

## But it’s not all science!

I also have a few personal projects that keep me busy:

- [**AURICLE:**](/_other_projects/auricle) My earring business, inspired by powerful women. I also donate earrings to survivors of sexual violence.
- [**Dogs of Harrison Park Calendar:**](/_other_projects/dog_calendar) Since 2017, I’ve organized a charity calendar supporting the Edinburgh Dog and Cat Home. I’m expanding this idea to help other communities raise money too.

<div class="bottomLinkTile">
  <a href="{{ '/other_projects' | relative_url }}">
    Go to Other Projects Page.
  </a>
</div>

<hr />

## When I’m not working, I’m probably:

- Out on adventures with my two dogs, Sid and Harry, exploring beautiful Scotland.
- Buried in a good book (mostly fantasy—[here’s what I’m reading now](reading_blog)).
- Collecting quirky salt and pepper shakers, because why not?
- Engrossed in a new creative hobby - crochet, lino cutting/ printing, watercolour, embroidery, ... (not that I'm particularly good at any of these things, but that's not the point) or experimenting with new recipes in the kitchen!
