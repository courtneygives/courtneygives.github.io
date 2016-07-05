---
layout: default
title: Drivel
permalink: /blog/
---

<h1>Latest nonsense...</h1>
  {% for post in site.posts limit:2 %}
  <h4 class="post-meta">{{ post.date | date: "%b %-d, %Y" }}:
  <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h4>
  <p>{{ post.content | strip_html | truncatewords:300}}</p>
  {% endfor %}

<ul class="posts">
  {% for post in site.posts limit:20 %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
        <span class="post-date">
          <span class="marker-dot-right"></span>
          {{ post.date | date: "%b %-d, %Y" }}
        </span>
        <span class="post-link">{{ post.title }}</span>
      </a>
    </li>
  {% endfor %}
</ul>
