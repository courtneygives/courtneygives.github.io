---
layout: page
title: Drivel
permalink: /blag/
---

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