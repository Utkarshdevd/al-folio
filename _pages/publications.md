---
layout: page
title: Publications
order: 1
permalink: /publications
description: Research papers resulting from collaborations from my time in undergraduate years at IIT Guwahati, IBM Research India, and now at University of Maryland.
nav: true
---

<div class="newprojects container mt-4">

  {% assign sorted_projects = site.publications | sort: "importance" %}
  {% for project in sorted_projects %}
  
  <div class="row mb-3">
    <!-- {% if project.redirect %}
    <a href="{{ project.redirect }}" target="_blank">
    {% else %}
    <a href="{{ project.url | relative_url }}">
    {% endif %} -->
      {% if project.img %}
      <div class="col-sm-3">
          <img class="img-fluid" src="{{ project.img | relative_url }}" alt="{{project.alttext}}">
      </div>
      {% endif %}
      <div class="col-sm-9">
          <h4 class="card-title">{{ project.title }}</h4>
          <p class="card-text">{{ project.description }}</p>
          {% if project.award %}
            <p class="purplecolor"> <i class="fas fa-trophy"></i> {{ project.award }}</p>
          {% endif %}
          <div class="row abbr ml-1 p-0 pubs">
           <div class="links">
                <a href="{{ project.pdf }}" class="btn btn-sm z-depth-0 m-0" role="button" target="_blank">{{project.type}} <i class="fas fa-download"></i></a>
                {% if project.abstract %}
                  <a class="abstract btn btn-sm z-depth-0" role="button">Abstract</a>
                {% endif %}
                </div>
                {% if project.abstract %}
                  <div class="abstract hidden">
                    <p>{{ project.abstract }}</p>
                  </div>
                {% endif %}

          </div>
          <div class="row ml-1 mr-1 p-0 pubs">
              
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
