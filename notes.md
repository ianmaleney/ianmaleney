---
layout: page
title: Notes
permalink: /notes/
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

<script>

  var blog_menu_items = document.querySelectorAll(".blog-menu__item");
  var blog_menu_posts = document.querySelector(".blog-menu__item--posts");
  var blog_menu_photos = document.querySelector(".blog-menu__item--photos");
  var blog_menu_links = document.querySelector(".blog-menu__item--links");
  var blog_sections = document.querySelectorAll(".blog_section");

  blog_menu_posts.addEventListener("click", function(){
    for(var i = 0; i < blog_sections.length; i++) {
      blog_sections[i].classList.remove("visible");
      blog_menu_items[i].classList.remove("active");
    }
    blog_sections[0].classList.add("visible");
    this.classList.add("active");
  });

  blog_menu_photos.addEventListener("click", function(){
    for(var i = 0; i < blog_sections.length; i++) {
      blog_sections[i].classList.remove("visible");
      blog_menu_items[i].classList.remove("active");
    }
    blog_sections[1].classList.add("visible");
    this.classList.add("active");
  });

  blog_menu_links.addEventListener("click", function(){
    for(var i = 0; i < blog_sections.length; i++) {
      blog_sections[i].classList.remove("visible");
      blog_menu_items[i].classList.remove("active");
    }
    blog_sections[2].classList.add("visible");
    this.classList.add("active");
  });

</script> 