---
layout: archive
title: "Educational Technology"
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

{% assign edtech = (site.posts | where: "category" , "edtech") %}
<ul>
  {% for post in edtech %}
    <li class="tile">
      <a href="{{ site.baseurl }}{{ post.url }}"><div class="post-teaser"><img src="{{ site.baseurl }}/images/{{ post.image.teaser }}" ></div>
      <div class="post-title">{{ post.title }}</div></a>
      <p class="post-excerpt">{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>