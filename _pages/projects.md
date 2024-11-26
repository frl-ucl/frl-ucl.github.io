---
layout: page
title: Research
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

        <p style="font-size: 25px;"><b>Vision-based</b></p>

        <p style="text-align: justify;">In collaboration with Port of London Authority, our research group conducted a series of data collection trials on the River Thames. We used multiple perception sensors including 3D LiDAR, high-resolution cameras, sound velocity profilers, etc. onboard a survey vessel to achieve a comprehensive autonomous understanding of traffic in busy waterways. We are grateful for the support from Port of London Authority and our funder, EPSRC.</p>

        <!-- This is an example post with videos. It supports local video files. -->

        <div class="row justify-content-sm-center">
            <!-- <div class="col-sm-8 mt-3 mt-md-0"> -->
            {% include video.liquid path="assets/img/projects/lidar-based.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
            <!-- </div> -->
        </div>

        <!-- References -->
        <!-- <div style="border: 1px solid black; padding: 10px; border-radius: 5px;"> -->
            <!-- <p>Research Output </p> -->
        <!-- </div> -->

        <br>

        <p style="font-size: 25px;"><b>LiDAR-based</b></p>

        <div class="row justify-content-sm-center">
            <div class="col-sm-8 mt-3 mt-md-0">
                {% include figure.liquid loading="eager" path="assets/img/projects/marina-still.gif" title="Marina Still" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>

    {% elsif category == "Intelligent Planning and Decision Making" %}
         <p style="text-align: justify;">We design intelligent planning algorithms that enable autonomous systems to make adaptive decisions in dynamic and unpredictable environments. By leveraging deep learning and optimization techniques, our work focuses on enhancing the ability of robots to navigate complex scenarios, efficiently allocate resources, and respond to changing conditions in real time. This ensures robust and reliable performance in challenging operational settings, from marine environments to urban spaces.</p>

        <p style="font-size: 25px;"><b>Path and Trajectory Planning</b></p>
        <div class="row justify-content-sm-center">
            <div class="col-sm-8 mt-3 mt-md-0">
                {% include figure.liquid loading="eager" path="assets/img/projects/usv-planning.gif" title="USV Planning" class="img-fluid rounded z-depth-1 half-width" %}
            </div>
        </div>


        <br>
        <p style="font-size: 25px;"><b>Task allocation for multi-robot systems</b></p>
        <div class="row justify-content-sm-center">
            <div class="col-sm-8 mt-3 mt-md-0">
                {% include figure.liquid loading="eager" path="assets/img/projects/task-planning.png" title="Task Planning" class="img-fluid rounded z-depth-1 half-width" %}
            </div>
        </div>


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