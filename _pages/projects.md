---
layout: page
title: Publications
permalink: /publications
description: Here are the papers I have published or are under review.
nav: true
---

<div class="newprojects container">

  {% assign sorted_projects = site.projects | sort: "importance" %}
  {% for project in sorted_projects %}
  
  <div class="row mb-3">
    <!-- {% if project.redirect %}
    <a href="{{ project.redirect }}" target="_blank">
    {% else %}
    <a href="{{ project.url | relative_url }}">
    {% endif %} -->
      {% if project.img %}
      <div class="col-sm-4">
          <img class="img-fluid" src="{{ project.img | relative_url }}" alt="project thumbnail">
      </div>
      {% endif %}
      <div class="col-sm-8">
          <h3 class="card-title">{{ project.title }}</h3>
          <p class="card-text">{{ project.description }}</p>
          <div class="row ml-1 mr-1 p-0">
            {% if project.github %}
            <div class="github-icon">
              <div class="icon" data-toggle="tooltip" title="Code Repository">
                <a href="{{ project.github }}" target="_blank"><i class="fab fa-github gh-icon"></i></a>
              </div>
              {% if project.github_stars %}
              <span class="stars" data-toggle="tooltip" title="GitHub Stars">
                <i class="fas fa-star"></i>
                <span id="{{ project.github_stars }}-stars"></span>
              </span>
              {% endif %}
            </div>
            {% endif %}
        </div>
      </div>
    <!-- </a> -->
  </div>
{% endfor %}

</div>
