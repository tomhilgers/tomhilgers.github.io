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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lorem ex, blandit vel ex sit amet, accumsan suscipit ante. Donec rutrum dolor id nisl blandit, quis cursus nunc sodales. Maecenas mollis, arcu quis elementum varius, metus justo varius justo, mollis porttitor ipsum neque eget risus. Aliquam erat volutpat. Mauris placerat sem nec felis auctor, eleifend vulputate lectus imperdiet. Donec at nunc quis tortor rhoncus 

Research Interests
------
- asdasd
- asdasdasd
 
Education
------
- **M.Sc. in Computer Science**
    - RWTH Aachen University, with distinction  
    - Thesis: *Coupling Turbulent Boundary Layer Flow Simulation with a Transformer*
    - January 2023 -- December 2025  
  
- **B.Sc. in Computer Science**
    - RWTH Aachen University
    - Thesis: *Designing a Static Performance Model and Code Generation for Vector Accelerators and Parallel Patterns*
    - October 2019 -- January 2023 

Supervision of Theses
------
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lorem ex, blandit vel ex sit amet, accumsan suscipit ante. Donec rutrum dolor id nisl blandit, quis cursus nunc sodales. Maecenas mollis, arcu quis elementum varius, metus justo varius justo, mollis porttitor ipsum neque eget risus. Aliquam erat volutpat. Mauris placerat sem nec felis auctor, eleifend vulputate lectus imperdiet. Donec at nunc quis tortor rhoncus 

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
