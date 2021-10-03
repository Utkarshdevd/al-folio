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
Utkarsh Dwivedi is currently enrolled in the Information Studies PhD program at University of Maryland, College Park (UMD). He obtained his Bachelors in Design in 2015 from the Indian Institute of Technology (IIT) at Guwahati. His current research focuses on Human-Computer Interaction, Applied Machine Learning, Educational Technologies and Accessibility. He is a Research Assistant at the <a href="https://iam.umd.edu/" target="_blank">Intelligent Assistive Machines (IAM) lab</a> at UMD led by <a href="https://scholar.google.com/citations?user=El-R5MEAAAAJ" target="_blank">Dr. Hernisa Kacorri</a> and <a href="https://www.researchgate.net/profile/Elizabeth-Bonsignore" target="_blank">Dr. Elizabeth Bonsignore</a>, the Director of <a href="https://hcil.umd.edu/children-as-design-partners/" target="_blank">KidsTeam</a> at UMD.
</p>

<p>You can download his <a href="/pdfs/Utkarsh_Dwivedi_CV_2021.pdf" download>CV</a> here.</p>

<h2 class="post-title">Experience</h2>
<div class="newprojects container">

  {% assign sorted_exp = site.experience | sort: "importance" %}
  {% for exp in sorted_exp %}
  
  <div class="row mb-3 d-flex flex-wrap align-items-center">
      {% if exp.img %}
      <div class="col-md-2 ">
          <img class="w-50 mx-auto d-block" src="{{ exp.img | relative_url }}" alt="exp thumbnail">
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
  
  <div class="row mb-3 d-flex flex-wrap align-items-center">
      {% if patent.img %}
      <div class="col-sm-2">
          <img class="w-50 mx-auto d-block" src="{{ patent.img | relative_url }}" alt="patent thumbnail">
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