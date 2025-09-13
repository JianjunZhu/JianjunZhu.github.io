---
permalink: /
title: "Academic Pages"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

Research Interests
====== 
Research Interests include the following categories:
* Medical Image Computing:
  * Algorithms for organs, structures, and lesions segmentation in multimodal medical imaging; Interventional planning based on multimodal imaging;  AI foundation models for cross-modal medical images.
* Computer Assisted Intervention:
  * Cross-modal medical image registration and fusion algorithms; Identification algorithms for various interventional instruments in intraoperative X-ray video; Image-based recognition of patients’ respiratory states and phases.
* Interventional Surgical Robotics:
  * Robot-assisted control (Co-pilot systems); Closed-loop robotic control based on fusion of multi-sensor information; Robotic AI agents.

Education
======
* Ph.D in Version Control Theory, GitHub University, 2018 (expected)
* M.S. in Jekyll, GitHub University, 2014
* B.S. in GitHub, GitHub University, 2012

Work experience
======
* Spring 2024: Academic Pages Collaborator
  * GitHub University
  * Duties includes: Updates and improvements to template
  * Supervisor: The Users

* Fall 2015: Research Assistant
  * GitHub University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub

* Summer 2015: Research Assistant
  * GitHub University
  * Duties included: Tagging issues
  * Supervisor: Professor Git
  
Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams
