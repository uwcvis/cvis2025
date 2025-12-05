---
title: Keynote Speakers
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: https://cvis2021.weebly.com/uploads/5/6/3/0/56308869/background-images/236520036.jpg
  actions:
permalink: /keynotes
toc: true
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
## {{ keynote.title }}
<img src="{{ keynote.image}}" class="align-left" style="width: calc(30% - 0.5em);"/>

{% if keynote.time %} <sub>{{keynote.time}} </sub>  {% endif %}


{% if keynote.url %} <sub> {{keynote.url}}</sub> {% endif %}

{% if keynote.abstract %}
**Abstract:** 
{{keynote.abstract}}
{% endif %}

**Speaker Info:**
{{keynote.author.name}}

{{keynote.author.description}}

{{keynote.author.bio}}

{% endfor %}
