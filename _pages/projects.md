---
layout: page
title: Projects
permalink: /projects/
description: Current and past projects that I have been a part. Click on each project to know more
nav: true
display_categories: [Current Work, Past Work]
horizontal: true
---
<div class="projects mt-4">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h3 class="category">{{category}}</h3>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <!-- Generate cards for each project -->

        <div class="container">
          <div class="row">
          {% for project in sorted_projects %}
            {% include projects_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      
    {% endfor %}

  {% else %}
  <!-- Display projects without categories -->
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <!-- Generate cards for each project -->
      <div class="container">
        <div class="row">
        {% for project in sorted_projects %}
          {% include projects_horizontal.html %}
        {% endfor %}
        </div>
      </div>

  {% endif %}

</div>
