---
title: "Talks and presentations"
excerpt: List of talks I have offered"
permalink: /talks/
---

<!-- Include the information you want to present at the top of the page here -->

This is a selective list of talks I have offered. You can find a more complete
list at my research platforms.

<!-- ######################################################################### -->
<!-- The code below creates the talk list from the contents of  -->
<!-- _data/talks.yml -->
<!-- Be careful when modifying its contents -->
<!-- ######################################################################### -->

{% for talk in site.data.talks %}

  <h3>
      {% if talk.url_or_doi %}
      <em><a href="{{ talk.url_or_doi }}">{{ talk.title }}</a></em>
      {% else %}
      {{ talk.title }}
      {% endif %}
  </h3> 
  <p>{{ talk.where }}, {{ talk.date }}</p>
  <p>{{ talk.description }}</p>
  {% if talk.authors %}
  <p>{{ talk.authors }}</p>
  {% endif %}
{% endfor %}
