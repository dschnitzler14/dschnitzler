---
layout: post
title: BlinkR Reflections
parent_project: 01_blinkr
---

I’ve come to realise how much I value taking stock and reflecting on a project once it reaches completion—or even an intermediate stage. So here are my reflections on the BlinkR project.

BlinkR wasn’t my first time working with Shiny, but it _was_ the first time I worked at this scale, the first time I used modularity, and the first Shiny project that actually reached completion.

My first foray into Shiny was a project that is still ongoing (if somewhat stalled), aimed at creating a Shiny companion app for a virtual statistical textbook developed by a colleague. I spent a day learning the basics and was thrilled that I could create something useful and visually appealing within just a few hours, despite never having used the framework before.

I identified a need for BlinkR while helping to plan a new university course designed to teach medical students the fundamentals of scientific research. The goal was to help them better understand the importance of research rigour and how to critically assess other studies for integrity and trustworthiness. We hit a roadblock when it came to the analysis component: we wanted the students to carry out their own analyses, not just observe results generated behind the scenes. But how could we facilitate this?

Do we ask them to download R and RStudio on their laptops? That assumes everyone has a laptop, which isn’t always the case. Many students only bring a tablet—or even just a phone—to class. Do we book a computer lab and pre-install everything on university machines? That felt complicated and less engaging. So I did some preliminary research: is there a way to run R virtually? The answer was yes!

So I set to work. I started with the analysis section and slowly built out the other components of the app, eventually going back to overhaul the early analysis section as well. The final product is an app that allows students to plan their experiment, gather data, analyse it, obtain results, and prepare for write-up—all within the app. It’s accessible from a smartphone, tablet, or computer. All you need is an internet connection!

Having previously dabbled in Shiny, I’d heard of modularity and liked the sound of it. I decided to build BlinkR using a modular architecture. This was my first real attempt at modularity, and I’ll admit I nearly gave up on it several times. It was tough to rethink everything I’d learned so far about Shiny to make it work with modules. As described in a public webinar by [Emily Riederer](https://youtu.be/F6I_jXPWFBk?si=fY5b_6B-aTKBLpNG), learning modules after learning the basics feels counterintuitive—and it is. But I can confirm that persevering was absolutely worth it. BlinkR became a large, complex app, and I shudder to think how chaotic and confusing it would’ve been had I stuck to the traditional `ui.R` and `server.R` structure. Some of the longer modules (which themselves contain nested modules) are over 1,000 lines long. A traditional structure would have meant managing a 10,000-line script. No thank you.

Once the analysis section was “good enough” to be used, we trialled it with a class. Yes, there were some hiccups, but the overall feedback delighted me. They thought it was fun! They thought it was cool! They thought it was useful! That spurred me on to continue—ironing out bugs and adding features to improve the student experience.

While I initially developed BlinkR for a specific course and audience, I always had a broader vision: to make it available to other educators. To support different experiments of similar design (e.g., comparing two groups), I took on the very tedious—but ultimately rewarding—task of replacing all hardcoded variables with dynamic ones that educators can define before deploying the app. This really stretched my thinking, as I had to consider how each variable was used across the UI, code editors, and server logic.

Here’s the bottom line: I learned the basics of Shiny in a day, but then took that knowledge apart to re-learn it at a more intermediate level (i.e., modules) in order to create something I’d never imagined I could. I became truly passionate about this project and genuinely enjoyed every second of it.

I’m incredibly proud of BlinkR and of everything I learned while building it. Without any formal education in coding or software development, I’ve come at this sideways—learning through trial and error. It’s pushed me to think deeply about the consequences of changing a module and how that affects the broader web of connections throughout the app. For me, BlinkR has been a _creative_ project, one filled with problem-solving, discovery, and joy.

If you're an expert developer reading this, you might think this is small potatoes—that “anyone can do this.” If that’s the case, then you’re lucky to have learned so much already. If you’re a beginner, like I was not long ago, remember: nobody wakes up just knowing things. Sometimes learning is easy, and sometimes it’s frustrating. Give yourself grace and take the time you need. Is it frustrating? Absolutely. Is it worth it? Only if you care about what you're doing. And if you’re not passionate about “it”—whether that’s the project or the skills you’re gaining—then don’t do it. I’m not trying to sound preachy—I just want to reassure anyone reading this: if I can do it, so can you. And maybe, in a few months, you’ll reflect on what you’ve learned, too. If you do, I’d love to read your reflection—whatever your project. Feel free to drop me a line.

Finally, the denouement of this reflection: am I a Shiny expert now? Probably not. But I would consider myself an advanced user. I look forward to building on what I’ve learned and working on fun, creative projects that challenge and frustrate me—and spark both passion and creativity in equal measure.
