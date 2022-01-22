---
layout: page
title: Projects
permalink: /projects/
description: A collection of some of my projects.
nav: true
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">

  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  <div class="container">
    <div class="row row-cols-3">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
    </div>
  </div>
</div>
