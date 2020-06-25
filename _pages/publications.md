---
title: "Publications"
excerpt: List of my publications"
permalink: /publications/
---

<!-- Include the information you want to present at the top of the page here -->

This is a selective list of my publications. You can find a more complete
list at my research platforms.


<!-- ######################################################################### -->
<!-- The code below creates the publication list from the contents of  -->
<!-- _data/publication.yml -->
<!-- Be careful when modifying its contents -->
<!-- ######################################################################### -->

{% for pub in site.data.publications %}

  <h3>
      {% if pub.url_or_doi %}
      <em><a href="{{ pub.url_or_doi }}">{{ pub.title }}</a></em>
      {% else %}
      {{ pub.title }}
      {% endif %}
  </h3> 
  <p>Published in {{ pub.where }}, {{ pub.date }}</p>
  <p>{{ pub.description }}</p>
  {% if pub.authors %}
  <p>{{ pub.authors }}</p>
  {% endif %}
{% endfor %}
