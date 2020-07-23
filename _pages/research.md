---
title: "Research"
excerpt: "My research projects"
permalink: /research/
layout: research

# Delete next lines if you prefer not to have a feature row
feature_row_title: Research Interests
feature_row:
  - image_path: /images/p1.jpg
    alt: "Research interest 1"
    title: "Research interest 1"
    excerpt:
        "This is a description of item 1"
  - image_path: /images/p1.jpg
    alt: "Research interest 2"
    title: "Research interest 2"
    excerpt:
        "This is a description of item 2"
  - image_path: /images/p1.jpg
    alt: "Research interest 3"
    title: "Research interest 3"
    excerpt:
        "This is a description of item 3"
# Delete the previous lines if you prefer not to have a feature row
---

Include any additional content relevant to your research  here.

<!-- Delete next line if you prefer not to have a feature row. -->
<br />
<br />
{% if page.feature_row %}
  {% include feature_row %}
{% endif %}
<!-- Delete previous lines if you prefer not to have a feature row. -->
