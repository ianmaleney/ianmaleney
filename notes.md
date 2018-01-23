---
layout: index-list
title: Notes
permalink: /notes/
---

<div class="blog_section blog_section__posts">
  {% for post in site.posts %}
    {% include article.html %}
  {% endfor %}
</div>