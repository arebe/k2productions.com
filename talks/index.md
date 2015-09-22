---
layout: archive
title: "Talks and Writing"
date: 
modified:
excerpt:
image:
  feature:
  teaser:
  thumb:
share: false
---

{% assign talks = (site.posts | where: "category" , "talks") %}
<ul>
  {% for post in talks %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>