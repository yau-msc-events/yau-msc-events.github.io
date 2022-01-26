---
layout: page
title: Seminars
---


- DC: Derived categories seminar

- EG: Enumerative geometry seminar 

- MS: Mirror symmetry working group


      <br>
      {% assign pages_list = site.pages | sort:"name" %}
      {% for node in pages_list %}
        {% if node.title != null %}
          {% if node.layout == "seminarpage" %}
            <a class="sidebar-nav-item{% if page.url == node.url %} active{% endif %}" href="{{ site.baseurl }}{{ node.url }}">{{ node.title }}</a>
          {% endif %}
        {% endif %}
      {% endfor %}
