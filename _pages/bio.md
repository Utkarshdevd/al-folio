---
layout: bio
title: Bio/CV
order: 3
permalink: /bio
description: 
nav: true
---

<div>
<p>
Utkarsh Dwivedi is currently enrolled in the Information Studies PhD program at University of Maryland, College Park (UMD). He obtained his bachelors in design in 2015 from the Indian Institute of Technology (IIT) at Guwahati. His current research focuses on human-computer interaction, applied machine learning, learning technologies and accessibility. He is a research assistant at the Intelligent Assistive Machines lab at UMD under the supervision of the Assistant Professor Hernisa Kacorri, and Assistant Research Scientist as well as the Director of KidsTeam, Elizabeth Bonsignore.
</p>

<p>You can download his CV <a href="/pdfs/Utkarsh_Dwivedi_CV.pdf" download>here</a>.</p>

<h2 class="post-title">Experience</h2>
<div class="newprojects container">

  {% assign sorted_exp = site.experience | sort: "importance" %}
  {% for exp in sorted_exp %}
  
  <div class="row mb-3">
      {% if exp.img %}
      <div class="col-md-2 text-center">
          <img class="w-50 " src="{{ exp.img | relative_url }}" alt="exp thumbnail">
      </div>
      {% endif %}
      <div class="col-md-10">
          <a href="{{ exp.link }}" target="_blank"><h4 class="card-title">{{ exp.title }}</h4></a>
          <h5 class="card-text">{{ exp.position }}</h5>
          <p class="card-text">{{ exp.description }}</p>
      </div>
    <!-- </a> -->
  </div>
{% endfor %}

</div>



<h2 class="post-title">Education</h2>
<div class="newprojects container">
  {% assign sorted_patents = site.education | sort: "importance" %}
  {% for patent in sorted_patents %}
  
  <div class="row mb-3">
      {% if patent.img %}
      <div class="col-sm-2 text-center">
          <img class="w-50" src="{{ patent.img | relative_url }}" alt="patent thumbnail">
      </div>
      {% endif %}
      <div class="col-sm-10">
          <a href="{{ patent.link }}" target="_blank"><h4 class="card-title">{{ patent.title }}</h4></a>
          <h5 class="card-text">{{ patent.position }}</h5>
          <p class="card-text">{{ patent.description }}</p>
      </div>
    <!-- </a> -->
  </div>
{% endfor %}
</div>