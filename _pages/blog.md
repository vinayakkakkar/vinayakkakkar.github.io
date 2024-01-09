---
layout: default
permalink: /blog/
title: blog
nav: true
nav_order: 1
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 5
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3  # The number of links after the current page
---
<div class="post">

  {% assign blog_name_size = site.blog_name | size %}
  {% assign blog_description_size = site.blog_description | size %}

  {% if blog_name_size > 0 or blog_description_size > 0 %}
    <div class="header-bar">
      <h1>{{ site.blog_name }}</h1>
      <h2>{{ site.blog_description }}</h2>
    </div>
  {% endif %}

  <div class="tag-category-list">
    <ul class="p-0 m-0">
      <li>
        <i class="fa-solid fa-hashtag fa-sm"></i> <a href="https://medium.com/@vinayakkakkar17/paving-success-the-dynamic-trio-of-hard-work-tech-and-smart-machines-a0ebf03e97db" target="_blank">Read the Blog</a>
      </li>
    </ul>
  </div>
</div>
