---
layout: research_project_post
title: BlinkR
tag: education
pillar: education
description: Educational tool for students to plan, run, and analyse an experiment
github_link: https://github.com/dschnitzler14/BlinkR
---
<div class="bottomLinkTile">
  <a href="{{ '/research_projects/01_blinkr_reflections' | relative_url }}">
    📖 Read my Reflections on BlinkR →
  </a>
</div>

<hr />

# About BlinkR

BlinkR is a web app written in Shiny for R, designed to help students plan, run, and analyse an experiment. It aims to teach the fundamentals of experimental design, good research practices, and basic statistical analysis in R.

The app runs entirely in R, and instead of relying on complex databases like SQL, it uses Google Sheets and Google Drive for persistent storage—making it more accessible and easier to manage.

Originally developed for an experiment comparing blinks per minute under stressed and control conditions (hence the name), BlinkR is now generalisable to any experiment comparing two groups.

BlinkR can be used for experiments that compare two groups via a T-test or Wilcoxon signed-rank test (depending on normality), with three technical replicates. It supports both paired and unpaired data.

