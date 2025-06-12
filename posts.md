---
layout: default
title:  "All Posts"
date:   2025-06-13 00:16:00 +0330
categories: about
---

<h1>All Posts</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p>{{ post.excerpt }}</p>
      <small>Published on {{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
