---
layout: page
title: Experience
permalink: /experience
description: 
nav: true
---

<div class="newprojects container">

  {% assign sorted_exp = site.experience | sort: "importance" %}
  {% for exp in sorted_exp %}
  
  <div class="row mb-3">
      {% if exp.img %}
      <div class="col-sm-4 text-center">
          <img class="w-50" src="{{ exp.img | relative_url }}" alt="exp thumbnail">
      </div>
      {% endif %}
      <div class="col-sm-8">
          <a href="{{ exp.link }}" target="_blank"><h3 class="card-title">{{ exp.title }}</h3></a>
          <h5 class="card-text">{{ exp.position }}</h5>
          <p class="card-text">{{ exp.description }}</p>
      </div>
    <!-- </a> -->
  </div>
{% endfor %}

</div>
