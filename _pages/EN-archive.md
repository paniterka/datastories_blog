---
title: "In English"
permalink: /en/
author_profile: true
---


<div class="grid__wrapper">
  {% assign collection = 'en' %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>