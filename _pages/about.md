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
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lorem ex, blandit vel ex sit amet, accumsan suscipit ante. Donec rutrum dolor id nisl blandit, quis cursus nunc sodales. Maecenas mollis, arcu quis elementum varius, metus justo varius justo, mollis porttitor ipsum neque eget risus. Aliquam erat volutpat. Mauris placerat sem nec felis auctor, eleifend vulputate lectus imperdiet. - Donec at nunc quis tortor rhoncus 

Supervision of Theses
------
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lorem ex, blandit vel ex sit amet, accumsan suscipit ante. Donec rutrum dolor id nisl blandit, quis cursus nunc sodales. Maecenas mollis, arcu quis elementum varius, metus justo varius justo, mollis porttitor ipsum neque eget risus. Aliquam erat volutpat. Mauris placerat sem nec felis auctor, eleifend vulputate lectus imperdiet. Donec at nunc quis tortor rhoncus 

******

Publications
======


  <article class="publication">
    <div class="publication-content">
      <h3 class="publication-title"> Paper A </h3>
      <p class="publication-authors"> asd asd as</p>
      <div class="publication-venue"> as as </div>
      <div class="publication-links"> asdas </div>
    </div>
  </article>

  Paper A
  ------
  Author

  Conf

  


 {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}


  <div class="pub-entry">
    <div class="pub-number">
      {{ forloop.index }}
    </div>

    <div class="pub-content">
      <div class="pub-title">
        {{ post.title }}
      </div>

      <div class="pub-authors">
        {{ post.authors }}
      </div>

      <div class="pub-venue">
        {{ post.venue }} ({{ post.year }})
      </div>

      <div class="pub-links">
        {% if post.paperurl %}
          <a href="{{ post.paperurl }}">PDF</a>
        {% endif %}
        {% if post.doi %}
          <a href="https://doi.org/{{ post.doi }}">DOI</a>
        {% endif %}
        {% if post.citation %}
          <button onclick="toggleCitation('{{ forloop.index }}')">Cite</button>
        {% endif %}
      </div>

      {% if post.citation %}
        <div id="cite-{{ forloop.index }}" style="display:none;">
          {{ post.citation }}
        </div>
      {% endif %}
    </div>
  </div>
