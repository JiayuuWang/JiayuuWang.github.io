---
layout: default
title: "Blogs"
permalink: /blogs/
author_profile: true
---

<span class='anchor' id='blogs'></span>

# Blog Posts

<div class="blog-list">
{% for post in site.posts %}
  <div class="blog-box">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="blog-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
      {% if post.categories %}
      • 
      {% for category in post.categories %}
        <span class="blog-category">{{ category }}</span>{% unless forloop.last %}, {% endunless %}
      {% endfor %}
      {% endif %}
    </p>
    <p class="blog-excerpt">{{ post.excerpt | strip_html | truncate: 200 }}</p>
    <p><a href="{{ post.url }}">Read more →</a></p>
  </div>
{% endfor %}
</div>
