---
layout: page
title: Current Deals
permalink: /deals/
icon: loyalty
---

<div class="container">
  {% for post in site.posts limit:1 %}
    <h3><a href="#dealbtn">{{ post.title }}</a></h3>

    <!-- Modal Structure -->
    <div id="dealbtn" class="modal">
      <div class="modal-content">
        <h3>{{ post.title }}</h3>
        <p>{{ post.content }}</p>
      </div>
      <div class="modal-footer">
        <a href="#!" class=" modal-action modal-close waves-effect waves-green btn-flat">Close</a>
      </div>
    </div>
  {% endfor %}
</div>
