---
title: Keynote Speakers
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: https://cvis2021.weebly.com/uploads/5/6/3/0/56308869/background-images/236520036.jpg
  actions:
permalink: /keynotes
toc: true
toc_label: "Speakers"
toc_icon: "microphone"
keynotes:
  - title: Artificial Intelligence for Music, from Audio to Video, from Cyber to Physical
    time: Dec 15th 2:15pm-3:00pm
    url: 
    image: assets/images/bio-photo.jpg
    abstract: Abs.
    author: 
      name: Prof. Yuchen Cui
      description:
      bio: Bio.
  - title: 3D Computer Vision and its evolution from depth sensors to novel view synthesis 
    time: Dec 2nd 1pm-2pm
    url: https://theialab.ca 
    image: assets/images/bio-photo.jpg
    abstract: Abs.
    author: 
      name: Prof. Andrea Tagliasacchi 
      description: 
      bio: Bio. 
  - title: Winter Is Coming - Extending Self-Driving Perception to Adverse Weather
    time: Dec 3rd 11am-12pm
    url:
    image: assets/images/bio-photo.jpg
    abstract: Abs.
    author:
      name: Prof. Steven Waslander
      description: 
      bio: Bio.
  - title: Digital Pathology Meets Spatial Omics - Emerging Problems in Data Integration, Solutions, and New Opportunities 
    time: Dec 3rd 1pm-2pm 
    url: 
    image: assets/images/bio-photo.jpg
    abstract: Abs.
    author:
      name: Prof. Pinaki Sarder
      description: 
      bio: Bio.
---

{% for keynote in page.keynotes %}
<div class="keynote-section">
  <h2 class="keynote-title">{{ keynote.title }}</h2>
  
  <div class="keynote-meta">
    {% if keynote.time %}
    <div class="keynote-time">{{ keynote.time }}</div>
    {% endif %}
    {% if keynote.url %}
    <div class="keynote-link"><a href="{{ keynote.url }}" target="_blank" rel="noopener noreferrer">{{ keynote.url }}</a></div>
    {% endif %}
  </div>

  <div class="keynote-content">
    <div class="keynote-image-wrapper">
      <img src="{{ keynote.image | relative_url }}" alt="{{ keynote.author.name }}" class="keynote-image">
    </div>
    
    <div class="keynote-details">
      <div class="keynote-speaker">
        <h4 class="speaker-name">{{ keynote.author.name }}</h4>
        {% if keynote.author.description %}
        <p>{{ keynote.author.description }}</p>
        {% endif %}
      </div>

      {% if keynote.abstract %}
      <div class="keynote-abstract">
        <h4>Abstract</h4>
        <p>{{ keynote.abstract }}</p>
      </div>
      {% endif %}

      {% if keynote.author.bio %}
      <div class="keynote-bio">
        <h4>Biography</h4>
        <p>{{ keynote.author.bio }}</p>
      </div>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}
