---
layout: page
title: Mihir Sriram Aranala, GISP
subtitle: Transit planner with a quest for data
---

<div class="container hero">
  <div class="image">
    <img src="https://mihiraranala.github.io/assets/img/Mihir Sriram Aranala Headshot.jpg" alt="Mihir Sriram Aranala" class="hero-photo">
  </div>
  <div class="content">
    <p class="hero-lede">I am an architect and urban planner turned transit data analyst, currently pursuing an MBA in Finance &amp; Entrepreneurship at Westcliff University. I spent a semester in Umeå, Sweden studying Swedish architecture and urban design before landing in transit planning &mdash; where my work now sits at the intersection of rail, transit, and urban data.</p>
    <div class="cta-row">
      <a class="btn-cta btn-cta-primary" href="#gallery">View My Work</a>
      <a class="btn-cta btn-cta-secondary" href="Mihir_Resume_July_2026.pdf">Resume</a>
    </div>
  </div>
</div>

<div class="stat-strip">
  <span class="stat-badge">GISP Certified</span>
  <span class="stat-badge">AECOM &middot; Transportation Planner</span>
  <span class="stat-badge">MS Urban &amp; Environmental Planning, ASU</span>
  <span class="stat-badge">B.Arch, Manipal Academy of Higher Education</span>
</div>

<p class="hero-extra">👀 Interested in the intersection of Transport (Rail and Transit) and urban data &nbsp;&middot;&nbsp; 📫 <a href="mailto:mihir.planning@gmail.com">mihir.planning@gmail.com</a></p>

## Maps Highlighted at ESRI UC 2026 Map Gallery - July 2026

<img src="https://mihiraranala.github.io/assets/img/ESRI-UC-1.jpg" alt="Mihir Aranala's maps selected for ESRI UC 2026" width="500"> <br>
Mihir Aranala's map was selected for the Map Gallery at ESRI UC 2026.


## Arizona Forward Emerging Sustainability Leaders Program - May 2026

<img src="https://mihiraranala.github.io/assets/img/AZF_ESL_Graduation_1.jpg" alt="Mihir Aranala graduates from the Arizona Forward Emerging Sustainability Leaders Program" width="500"> <br>
Mihir Aranala graduated from the Emerging Sustainability Leaders Program conducted by Arizona Forward.


## Arizona Forward Emerging Sustainability Leaders Program - September 2025

<img src="https://arizonaforward.org/wp-content/uploads/2025/09/2025-2026-Emerging-Sustainability-Leaders.jpg" alt="Mihir Aranala - Arizona Forward Emerging Sustainabiltiy Leaders" width="500"/> <br>
Mihir Aranala was selected for the Emerging Sustainability Leaders Program conducted by Arizona Forward.

<a class="link-text" href="https://acrobat.adobe.com/id/urn:aaid:sc:US:3747fa45-b573-4a9b-9a86-5a5274be78dd"> Meet the Program Cohort</a>


## AGIC Symposium Presentation - August 2025

<img src="https://mihiraranala.github.io/assets/img/mihir-aranala-presentation.png" alt="Mihir Aranala - AGIC Presentation" width="500"/> <br>
Mihir Aranala presented at the Arizona Geographic Information Council Training Symposium 2025.

<a class="link-text" href="https://storymaps.arcgis.com/stories/06baa0c0a6714e20b4167ae9ac08d468"> Check out the AGIC Q4 Newsletter</a>

## GIS Chat Podcast - November 2024

<img src="https://www.buzzsprout.com/rails/active_storage/representations/redirect/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBCSGJOc0FVPSIsImV4cCI6bnVsbCwicHVyIjoiYmxvYl9pZCJ9fQ==--418e44dea1dfa1833563662af194b12e77877435/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdDVG9MWm05eWJXRjBPZ2hxY0djNkUzSmxjMmw2WlY5MGIxOW1hV3hzV3docEFsZ0NhUUpZQW5zR09nbGpjbTl3T2d0alpXNTBjbVU2Q25OaGRtVnlld1k2REhGMVlXeHBkSGxwUVRvUVkyOXNiM1Z5YzNCaFkyVkpJZ2x6Y21kaUJqb0dSVlE9IiwiZXhwIjpudWxsLCJwdXIiOiJ2YXJpYXRpb24ifX0=--1924d851274c06c8fa0acdfeffb43489fc4a7fcc/1.jpg" alt="Jazzmen Wilson - GIS Chat Podcast" width="200"/> <br>
Check out my latest podcast episode where I share my journey from being an intern to a full-time Transportation Planner at AECOM. I talk about the importance of public transit and how my experiences in India have shaped my drive journey. Tune in for an insightful conversation!


<a class="link-text" href="https://open.spotify.com/episode/0GOUR0gQFtYmXB2iquE971"> Spotify</a>
<a class="link-text" href="https://podcasts.apple.com/us/podcast/mihir-aranala/id1712968933?i=1000675874793">Apple Podcasts</a>


{% assign posts = site.tags['projects'] %}
{% assign featured = posts | first %}

## Selected Projects {#gallery}

{% if featured %}
  {%- capture featured_thumb -%}
    {% if featured.thumbnail-img %}
      {{ featured.thumbnail-img }}
    {% elsif featured.cover-img %}
      {% if featured.cover-img.first %}
        {{ featured.cover-img[0].first.first }}
      {% else %}
        {{ featured.cover-img }}
      {% endif %}
    {% else %}
    {% endif %}
  {%- endcapture -%}
  {% assign featured_thumb = featured_thumb | strip %}

  {% if featured_thumb != "" %}
  <div class="featured-project">
    <a class="featured-project-img" href="{{ featured.url | absolute_url }}">
      <img src="{{ featured_thumb | absolute_url }}" alt="{{ featured.title | strip_html }}">
    </a>
    <div class="featured-project-info">
      <span class="featured-label">Featured Project</span>
      <h3><a href="{{ featured.url | absolute_url }}">{{ featured.title | strip_html }}</a></h3>
      {% if featured.subtitle %}<p class="featured-subtitle">{{ featured.subtitle | strip_html }}</p>{% endif %}
      <p class="featured-excerpt">{{ featured.excerpt | strip_html | truncatewords: 30 }}</p>
    </div>
  </div>
  {% endif %}
{% endif %}

<div class="gallery">
  {% for post in posts offset: 1 %}
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
        <img src="{{ thumbnail | absolute_url }}" alt="{{ post.title | strip_html }}">
        <span class="gallery-caption">{{ post.title | strip_html }}</span>
      </a>
    </div>
    {% endif %}
  {% endfor %}
</div>
