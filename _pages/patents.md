---
layout: page
title: Patents
permalink: /patents
order: 2
description: Patents that I have filed, during my time at IBM Research India.
nav: true
---

<div class="patents container">

  {% assign sorted_patents = site.patents | sort: "importance" %}
  {% for patent in sorted_patents %}
  
  <div class="row mb-3">
      {% if patent.img %}
      <div class="col-sm-4 text-center">
          <img class="w-50" src="{{ patent.img | relative_url }}" alt="patent thumbnail">
      </div>
      {% endif %}
      <div class="col-sm-8">
          <a href="{{ patent.link }}" target="_blank"><h3 class="card-title">{{ patent.title }}</h3></a>
          <h5 class="card-text">{{ patent.authors }}</h5>
          <p class="card-text">{{ patent.description }}</p>
          <div class="row ml-1 mr-1 p-0">
            <a href="{{ patent.link }}" class="btn btn-sm z-depth-0 m-0" role="button" target="_blank">{{ patent.patentid }}</a>
        </div>
      </div>
    <!-- </a> -->
  </div>
{% endfor %}

</div>
