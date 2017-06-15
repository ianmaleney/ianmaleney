---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog_section blog_section__posts visible">
  {% assign blogposts = site.posts | where: "category","blog_post" %}
  {% for post in blogposts %}
    {% include article.html %}
  {% endfor %}
</div>

<div class="blog_section blog_section__photos">
	{% assign blogphotos = site.posts | where: "category","blog_photos" %}
  {% for post in blogphotos %}
    {% include article.html %}
  {% endfor %}
 </div>
<div class="blog_section blog_section__links">
	{% assign bloglinks = site.posts | where: "category","blog_links" %}
  {% for post in bloglinks %}
    {% include article.html %}
  {% endfor %}
</div>

<ul class="blog-menu">
  <li class="blog-menu__item blog-menu__item--posts active">Posts</li>
  <li class="blog-menu__item blog-menu__item--photos">Photos</li>
  <li class="blog-menu__item blog-menu__item--links">Links</li>
</ul>