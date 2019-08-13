---
title: "Posts in English"
permalink: /EN/
author_profile: true
truncatewords: 150 
---


## Latest stories

<div class="grid__wrapper">
  {% assign collection = 'EN' %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>