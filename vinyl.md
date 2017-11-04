---
layout: default
title: Vinyl
permalink: /vinyl/
---
<ul class="post-list">
  {% assign posts = site.posts | where: "type", "vinyl" %}
  {% for post in posts %}
    <li class="post">
      <h2 class="post-header">
        {{ post.title | escape }}
      </h2>
      <div>
        {{ post.content }}
      </div>
      <img class="post-image" src="{{ post.image_url }}" />
    </li>
  {% endfor %}
</ul>
