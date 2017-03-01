---
layout: page
title: Current Deals
permalink: /deals/
icon: loyalty
---

<div class="container">
  {% for post in site.posts limit:1 %}
    <h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
    <time>{{ post.date | date: "%b %-d, %Y" }}</time>
  {% endfor %}
</div>
