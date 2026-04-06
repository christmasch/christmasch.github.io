---
layout: page
permalink: /Research/
title: Research
description:
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<div class="publications">
  <h2>Working Papers</h2>
  {% bibliography --query @*[status=working-paper] %}

  <h2>Work in Progress</h2>
  {% bibliography --query @*[status=work-in-progress] %}
</div>
