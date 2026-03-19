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
Since April 2026, I am a researcher and Ph.D. student at the Chair for High Performance Computing at RWTH Aachen University. I graduated with an M.Sc. in 2026 and with a B.Sc. in 2023, both from RWTH Aachen University.

Research Interests
------
- Energy Efficient Machine Learning
- Machine Learning in Science
- TBD ...
 
Education
------
- **M.Sc. in Computer Science**
    - RWTH Aachen University, with distinction  
    - Thesis: *Coupling Turbulent Boundary Layer Flow Simulation with a Transformer*
    - 2023 -- 2025  
  
- **B.Sc. in Computer Science**
    - RWTH Aachen University
    - Thesis: *Designing a Static Performance Model and Code Generation for Vector Accelerators and Parallel Patterns*
    - 2019 -- 2023 

Supervision of Theses
------
Please inquire via <a href="mailto:contact@hpc.rwth-aachen.de">contact@hpc.rwth-aachen.de</a> for currently available thesis topics or to propose your own. Please include a short list of your interests, prior experience and transcript of records.

******

Publications
======

<ul>
  {% for post in site.publications reversed %}      
     <li>
        <h3 class="publication-title"> {{ post.title }}</h3>
        <div class="publication-authors"> {{ post.authors }}</div>
        <div class="publication-venue"> {{ post.venue }}, {{ post.year }} </div>
        <div class="publication-links"> 
          {% if post.paperurl %}
            <a href="{{post.paperurl}}" target="_blank" rel="noopener noreferrer">[PDF]</a>  
          {% endif %}
          {% if post.doi %}
            <a href="https://doi.org/{{post.doi}}" target="_blank" rel="noopener noreferrer">[DOI]</a>  
          {% endif %}
          {% if post.code %}
            <a href="{{post.code}}" target="_blank" rel="noopener noreferrer">[Code]</a>  
          {% endif %}
          {% if post.bibtex %}
            <details>
              <summary>[BibTeX]</summary>
              {{post.bibtex}}
            </details>  
          {% endif %}
        </div>
     </li>
  {% endfor %}   
</ul>
