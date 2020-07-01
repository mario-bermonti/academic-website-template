---
layout: home
author_profile: true
permalink: /
title: Welcome!

# Delete next lines if you prefer not to have a feature row
feature_row_title: Academic Interests
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
---

Include a long description about yourself and this website.




<!-- Delete next line if you prefer not to have a feature row. -->
<br />
<br />
{% if page.feature_row %}
  {% include feature_row %}
{% endif %}
