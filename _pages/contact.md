---
layout: page
title: Contact
permalink: /contact/
# description: "To reach our group for any enquiries or openings, please contact:"
nav: true
nav_order: 8
display_categories: [For Prospective PhD Students/Postdocs/Visiting Scholars, For General Enquiries] 
---

<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized sections -->
  {% for category in page.display_categories %}
    <a id="{{ category }}" href=".#{{ category }}">
      <h2 class="category">{{ category }}</h2>
    </a>
    <!-- Display text for each category -->
    {% if category == "For Prospective PhD Students/Postdocs/Visiting Scholars" %}
      <p>If you are interested in a PhD/post-doc position/visiting scholar position, please submit this <a href="https://forms.office.com/e/mTC2qZGhQM" target="_blank" style="text-decoration: underline;">form</a>.</p>
    {% elsif category == "For General Enquiries" %}
      <p>If you are interested in our projects or have general questions, please submit this <a href="https://forms.office.com/e/wbXeBDH32c" target="_blank" style="text-decoration: underline;">form</a>.</p>
    {% endif %}
  {% endfor %}
{% endif %}
</div>
