---
layout: page
permalink: /Research/
title: Research
description:
nav: true
nav_order: 2
---

<style>
/* Hide the large page title, but keep title: Research for the navigation */
.post-title {
  display: none;
}

/* Remove the automatically inserted bibliography year headings */
.publications h2.bibliography {
  display: none;
}

/* Remove empty image/preview area next to each paper */
.publications .preview {
  display: none !important;
}

/* Make each bibliography entry full width and create space for bullet */
.publications .bibliography .row {
  display: block;
  position: relative;
  padding-left: 1.2em;
  margin-bottom: 1.2em;
}



/* Let the publication text take the full width */
.publications .bibliography .col-sm-2,
.publications .bibliography .col-sm-8,
.publications .bibliography .col-sm-10 {
  max-width: 100%;
  flex: 0 0 100%;
  padding-left: 0;
}

/* Remove extra left/right Bootstrap padding */
.publications .bibliography .row > div {
  padding-left: 0;
  padding-right: 0;
}

/* More distance between Working Papers and Work in Progress */
.publication-section-spacer {
  height: 2rem;
}
</style>

<!-- _pages/publications.md -->

<div class="publications">
  <h2>Working Papers</h2>
  {% bibliography --query @*[status=working-paper] %}

  <div class="publication-section-spacer"></div>

  <h2>Work in Progress</h2>
  {% bibliography --query @*[status=work-in-progress] %}
</div>
