---
layout: page
permalink: /Research/
title: Research
description:
nav: true
nav_order: 2
---

<style>
.post-title {
  display: none;
}

/* Remove empty image/preview area next to each paper */
.publications .preview {
  display: none !important;
}

/* Let the publication text take the full width */
.publications .bibliography .row {
  display: block;
}

.publications .bibliography .col-sm-2,
.publications .bibliography .col-sm-8,
.publications .bibliography .col-sm-10 {
  max-width: 100%;
  flex: 0 0 100%;
}
</style>

<!-- _pages/publications.md -->

<div class="publications">
  <h2>Working Papers</h2>
  {% bibliography --query @*[status=working-paper] %}

  <h2>Work in Progress</h2>
  {% bibliography --query @*[status=work-in-progress] %}
</div>
