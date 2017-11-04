---
layout: default
title: Tshirts
permalink: /tshirts/
---
<ul class="post-list">
  {% assign posts = site.posts | where: "type", "tshirt" %}
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
