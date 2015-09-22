---
layout: archive
title: "Multimedia"
date: 
modified:
excerpt:
image:
  feature:
  teaser:
  thumb:
ads: false  
share: false
---

{% assign multimedia = (site.posts | where: "category" , "multimedia") %}
<ul>
  {% for post in multimedia %}
    <li class="tile">
      <a href="{{ post.url }}"><div class="post-teaser"><img src="{{ site.url }}/images/{{ post.image.teaser }}" ></div>
      <div class="post-title">{{ post.title }}</div></a>
      <p class="post-excerpt">{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
