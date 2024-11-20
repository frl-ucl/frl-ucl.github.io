---
layout: page
title: Projects
permalink: /projects/
description:  #"Our group is dedicated to advancing autonomous systems through cutting-edge research in three core areas: Reliable Sensing and Perception, Intelligent Planning and Decision Making, and Advanced Robust Control. Our mission is to develop resilient technologies that enhance system reliability by integrating sophisticated sensing, perception, and adaptive control frameworks. By leveraging the latest advances in machine learning, optimization, and control theory, we address real-world challenges, enabling autonomous platforms to navigate and operate effectively in complex, dynamic environments."
nav: true
nav_order: 3
display_categories: [Reliable Sensing and Perception, Intelligent Planning and Decision Making] #, Advanced Robust Control]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
   <!-- Display text for each category -->
    {% if category == "Reliable Sensing and Perception" %}
      <p style="text-align: justify;">We develop deep learning algorithms for robust object detection in challenging marine environments, enabling reliable perception under varying sea states, lighting conditions, and complex port settings. Our work focuses on enhancing the accuracy of underwater and surface object detection, ensuring the safe and efficient operation of autonomous maritime systems.</p>
    {% elsif category == "Intelligent Planning and Decision Making" %}
      <p style="text-align: justify;">We design intelligent planning algorithms that enable autonomous systems to make adaptive decisions in dynamic and unpredictable environments. By leveraging deep learning and optimization techniques, our work focuses on enhancing the ability of robots to navigate complex scenarios, efficiently allocate resources, and respond to changing conditions in real time. This ensures robust and reliable performance in challenging operational settings, from marine environments to urban spaces.</p>
    {% endif %}
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row justify-content-center">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row justify-content-center">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>