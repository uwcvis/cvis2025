---
title: Keynotes
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: https://cvis2021.weebly.com/uploads/5/6/3/0/56308869/background-images/236520036.jpg
  actions:
permalink: /keynotes
toc: true
keynotes:
  - title: Sorin Cheran
    time: 
    url: 
    image: \assets\images\sorincheran.jpeg
    abstract: 
    author: 
      name:
      description:
      bio: Sorin currently works in the Artificial Intelligence (AI) Lab at Hewlett Packard Labs. In his 12 years with HPE, Sorin has held a number of different roles. Until recently, he worked in the High-Performance Computing (HPC) and AI Competency Center in Grenoble, France as part of the Hybrid IT BU Presales team. Sorin’s career advancement has rapidly progressed from HPC Post-Sales Engineer to a customerfacing presales role and later, to Distinguished Technologist.  
  - title: Prof. Steven Waslander
    time:
    url:
    image: assets\images\steve-waslander.webp
    abstract:
    author:
      name: 
      description: 
      bio: Prof. Steven Waslander is a leading authority on autonomous aerial and ground vehicles, including multirotor drones and autonomous driving vehicles. Simultaneous Localization and Mapping (SLAM) and multi-vehicle systems. He received his B.Sc.E.in 1998 from Queen’s University, his M.S. in 2002 and his Ph.D. in 2007, both from Stanford University in Aeronautics and Astronautics, where as a graduate student he created the Stanford Testbed of Autonomous Rotorcraft for Multi-Agent Control (STARMAC), the world’s most capable outdoor multi-vehicle quadrotor platform at the time. He was a Control Systems Analyst for Pratt & Whitney Canada from 1998 to 2001. He was recruited to Waterloo from Stanford in 2008, where he founded and directs the Waterloo Autonomous Vehicle Laboratory (WAVELab), extending the state of the art in autonomous drones and autonomous driving through advances in localization and mapping, object detection and tracking, integrated planning and control methods and multi-robot coordination. In 2018, he joined the University of Toronto Institute for Aerospace Studies (UTIAS), and founded the Toronto Robotics and Artificial Intelligence Laboratory (TRAILab). He is an active member of the University of Toronto Robotics Institute, for which he acts as Chair of the Partner Consortium Committee.
  - title: Prof. Andrea Tagliasacchi
    time:
    url: 
    image: assets\images\andrea_tagliasacchi.jpeg
    abstract:
    author:
      name: 
      description: 
      bio: Andrea Tagliasacchi is an associate professor at Simon Fraser University (Vancouver, Canada) where he holds the appointment of Visual Computing Research Chair within the school of computing science. He is also a part-time (20%) staff research scientist at Google DeepMind (Toronto, Canada), as well as an associate professor (status only) in the computer science department at the University of Toronto. Before joining SFU, he spent four wonderful years as a full-time researcher at Google (mentored by Paul Lalonde, Geoffrey Hinton, and David Fleet). Before joining Google, he was an assistant professor at the University of Victoria (2015-2017), where he held the Industrial Research Chair in 3D Sensing (jointly sponsored by Google and Intel). His alma mater include EPFL (postdoc) SFU (PhD, NSERC Alexander Graham Bell fellow) and Politecnico di Milano (MSc, gold medalist). Several of his papers have received best-paper award nominations at top-tier graphics and vision conferences, and he is the recipient of the 2015 SGP best paper award, the 2020 CVPR best student paper award, and the 2024 CVPR best paper award (honorable mention). His research focuses on 3D visual perception, which lies at the intersection of computer vision, computer graphics and machine learning.

  - title: Prof. Pinaki Sarder
    time:
    url: 
    image: assets\images\Pinaki-Sarder.jpg
    abstract: 
    author:
      name: 
      description: 
      bio: Pinaki Sarder is currently an associate professor of AI in the Section of Quantitative Health of the Department of Medicine, as well as the Associate Director for Imaging in the Intelligent Critical Care Center at the University of Florida (UF). Before joining UF, he was an associate professor in the Departments of Pathology & Anatomical Sciences and Biomedical Engineering at the University at Buffalo (UB), where he was at the center of building the computationally enabled graduate program Computational Cell Biology, Anatomy, and Pathology. Prior to UB, he completed post-doctoral training at Mallinckrodt Institute of Radiology at the Washington University in St. Louis (WUSTL) School of Medicine. He received his B.Tech. degree in electrical engineering from the Indian Institute of Technology, Kanpur, in 2003, and M.Sc. and Ph.D. degrees in electrical engineering from WUSTL in 2010.
---


To be announced. 


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
