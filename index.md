---
layout: about
permalink: /
profile:
  align: right
  image: profile.png
published: true
---

<p>
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

<p>
  Latest Stuff and Nonsense: 
  {% assign latest_post = site.posts | first %}
  {{ latest_post.date | date: "%B, %Y" }} - 
  <a href="{{ latest_post.url | prepend: site.baseurl }}">{{ latest_post.title }}</a>
</p>

# Hey there! I'm Danny,

a post-doctoral researcher who loves blending science, coding, and creativity. I finished my PhD at the University of Edinburgh ([you can check it out here!](/research_projects/10_phd)) and now, I’m diving into new research at the Medical School Berlin with [Melanie Stefan](https://melaniestefan.net/){:target="\_blank"}. I’m all about learning and growing, and sharing my journey along the way.

I grew up in Vienna, Austria, but thanks to my American mum, I’ve always been fluent in English and German. In 2011, I made the leap to Scotland to study Biomedical Science at Aberdeen University. After graduating with my honours degree and integrated masters (MSci), I moved to Edinburgh to kick off my PhD, focusing on anxiety using a prenatal stress rat model. Through the course of my PhD I surprised myself and everyone around me when I really fell in love with coding.

## Right now, I’m:

- Exploring how English animal names compare to their evolutionary relationships ([check it out here](/_research_projects/01_tree_of_life)).
- Learning the foundations of machine learning to tackle a bigger project on bioimage analysis ([read more here](/_research_projects/01_bioimage)).
- Passionate about making science open and accessible, working on projects aimed at fixing some of the problems in scientific publishing ([more on that here](/_research_projects/01_paperstars))
- Looking at depression through an evolutionary lens ([read more here](/_research_projects/01_depression))

When I’m not deep in research, I love teaching and sharing knowledge. I'm contributing to the design of a course on the scientific process at the Medical School, as well as contributing to teaching (at least that's the plan), and I’m developing a cool interactive Shiny app to go along with a video textbook ([thoughts on that here](/_research_projects/01_stats_app)). I also get to co-supervise one of our amazing PhD students!

## But it’s not all science!

I also have a few personal projects that keep me busy:

- [**AURICLE:**](/_other_projects/auricle) My earring business, inspired by powerful women. I also donate earrings to survivors of sexual violence.
- [**Dogs of Harrison Park Calendar:**](/_other_projects/dog_calendar) Since 2017, I’ve organized a charity calendar supporting the Edinburgh Dog and Cat Home. I’m expanding this idea to help other communities raise money too.
- [**Lectures at Lunch:**](/_other_projects/lectures_at_lunch) Organizing virtual lunch talks for women across different fields, which is a great way to connect and share experiences.

## When I’m not working, I’m probably:

- Out on adventures with my two dogs, [Sid](https://www.instagram.com/sid_wags/){:target="\_blank"} and [Harry](https://www.instagram.com/harry.the.lamb/){:target="\_blank"}, exploring beautiful Scotland.
- Buried in a good book (mostly fantasy—[here’s what I’m reading now](reading_blog)).
- Collecting quirky salt and pepper shakers, because why not?
- Engrossed in a new creative hobby - crochet, lino cutting/ printing, watercolour, embroidery, ... (not that I'm particularly good at any of these things, but that's not the point) or experimenting with new recipes in the kitchen!
