---
title: "Po polsku"
permalink: /PL/
author_profile: true
---


## Latest stories

<div class="grid__wrapper">
  {% assign collection = 'PL' %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>