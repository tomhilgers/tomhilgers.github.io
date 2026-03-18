---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

About
=====


Research Interests
------

Education
------

Supervision of Theses
------

Publications
======

 {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
