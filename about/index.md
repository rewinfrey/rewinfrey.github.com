---
layout: default
title: About
---

<h1 class="page-heading">About</h1>

<ul class="posts">
  {% for post in site.posts %}
  <li>
  <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
  <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>