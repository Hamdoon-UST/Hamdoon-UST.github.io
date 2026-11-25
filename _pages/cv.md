---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======

* Ph.D. student, The Hong Kong University of Science and Technology
* M.Eng. in Aeronautical Science and Engineering (Fluid Mechanics), Beihang University, Beijing, China, 2019–2021
* B.Sc. in Mechanical Engineering, COMSATS University Islamabad, Pakistan, 2015–2019

Experience
======

* Ph.D. student, The Hong Kong University of Science and Technology
  * Research on the control of shallow-water waves with metamaterials
* Research and Development Engineer, Obrien Tech Limited, Hong Kong, 2022–2023

Skills
======

* Computational fluid dynamics
* Detached-eddy simulation and large-eddy simulation of separated flows
* Dynamic mode decomposition of unsteady vortex flows
* Nanofluid heat-transfer calculations for automotive cooling

Reviewing
======

* *Physics of Fluids* (AIP Publishing), 2026
* *Engineering Applications of Artificial Intelligence* (Elsevier), 2026
* *International Journal of Robust and Nonlinear Control* (WILEY), 2026

Publications
======

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Talks
======

<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

{% if site.talks.size == 0 %}
No talks are listed yet.
{% endif %}
