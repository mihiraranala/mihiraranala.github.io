---
layout: page
title: Mihir Aranala, GISP
subtitle: Transit planner with a quest for data
---

<img src="https://mihiraranala.github.io/assets/img/Mihir Sriram Aranala Headshot.jpg" width="200">

My name is Mihir Sriram Aranala. I am an architect and an urban planner by profession. I am currently pursuing my MBA in Finance and Entreprenuership.

Follow this link to my resume - <a class="link-text" href="Resume Mihir Aranala April 2024.pdf"> Here </a>


- I am a Transportation Planner at AECOM.
- I received my GISP certifcation in March 2025.
- My experience lies in data and spatial analysis, mapping, systems analysis, service and operations planning, and the use of various innovative tools.
- I assist in transit, microtransit, BRT, and bike planning through data, spatial analysis and report writing.
- I hold a Bachelor's degree in Architecture from Manipal Academy of Higher Education, India.
- I spent a semester in Umea, Sweden learning about Swedish architecture, urban design, and housing.
- I graduate from Arizona State University with a Masters' degree in Urban and Environmental Planning in May 2023.
- 👀 I’m interested in the intersection of Transport (Rail and Transit) and urban data.
- 📫 Email me at sriram.mihir@gmail.com


## Arizona Forward Emerging Sustainability Leaders Program - September 2025

<img src="https://arizonaforward.org/wp-content/uploads/2025/09/2025-2026-Emerging-Sustainability-Leaders.jpg" alt="Mihir Aranala - Arizona Forward Emerging Sustainabiltiy Leaders" width="500"/> <br>
Mihir Aranala was selected for the Emerging Sustainability Leaders Program conducted by Arizona Forward.

<a class="link-text" href="https://acrobat.adobe.com/id/urn:aaid:sc:US:3747fa45-b573-4a9b-9a86-5a5274be78dd"> Meet the Program Cohort</a>


## AGIC Symposium Presentation - August 2025

<img src="https://storymaps.arcgis.com/stories/06baa0c0a6714e20b4167ae9ac08d468" alt="Mihir Aranala - AGIC Presentation" width="500"/> <br>
Mihir Aranala presented at the Arizona Geographic Information Council Training Symposium 2025.

<a class="link-text" href="https://acrobat.adobe.com/id/urn:aaid:sc:US:3747fa45-b573-4a9b-9a86-5a5274be78dd"> Meet the Program Cohort</a>

## GIS Chat Podcast - November 2024

<img src="https://www.buzzsprout.com/rails/active_storage/representations/redirect/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBCSGJOc0FVPSIsImV4cCI6bnVsbCwicHVyIjoiYmxvYl9pZCJ9fQ==--418e44dea1dfa1833563662af194b12e77877435/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdDVG9MWm05eWJXRjBPZ2hxY0djNkUzSmxjMmw2WlY5MGIxOW1hV3hzV3docEFsZ0NhUUpZQW5zR09nbGpjbTl3T2d0alpXNTBjbVU2Q25OaGRtVnlld1k2REhGMVlXeHBkSGxwUVRvUVkyOXNiM1Z5YzNCaFkyVkpJZ2x6Y21kaUJqb0dSVlE9IiwiZXhwIjpudWxsLCJwdXIiOiJ2YXJpYXRpb24ifX0=--1924d851274c06c8fa0acdfeffb43489fc4a7fcc/1.jpg" alt="Jazzmen Wilson - GIS Chat Podcast" width="200"/> <br>
Check out my latest podcast episode where I share my journey from being an intern to a full-time Transportation Planner at AECOM. I talk about the importance of public transit and how my experiences in India have shaped my drive journey. Tune in for an insightful conversation!


<a class="link-text" href="https://open.spotify.com/episode/0GOUR0gQFtYmXB2iquE971"> Spotify</a>
<a class="link-text" href="https://podcasts.apple.com/us/podcast/mihir-aranala/id1712968933?i=1000675874793">Apple Podcasts</a>


{% assign posts = site.tags['projects'] %}

## Gallery Section

<div class="gallery">
  {% for post in posts %}
    {%- capture thumbnail -%}
      {% if post.thumbnail-img %}
        {{ post.thumbnail-img }}
      {% elsif post.cover-img %}
        {% if post.cover-img.first %}
          {{ post.cover-img[0].first.first }}
        {% else %}
          {{ post.cover-img }}
        {% endif %}
      {% else %}
      {% endif %}
    {% endcapture %}
    {% assign thumbnail=thumbnail | strip %}

    {% if thumbnail != "" %}
    <div class="gallery-item">
      <a href="{{ post.url | absolute_url }}">
        <img src="{{ thumbnail | absolute_url }}" alt="Project image">
      </a>
    </div>
    {% endif %}
  {% endfor %}
</div>
