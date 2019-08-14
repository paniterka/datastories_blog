---
title: "Posts by Tag"
permalink: /tags_collections/
author_profile: true
---

<!--
<div class="grid__wrapper">
{% for c in site.collections %}
  {% if c.label !='posts' %}
  <h1>{{ c.label }}</h1>
  {% assign collection = c.label %}
  {% assign posts = site[collection] | reverse %}
  {% for post in posts %}
    {% include archive-single.html type="list" %}
  {% endfor %}
  {% endif %}
{% endfor %}
</div>
-->


{% assign tags =  site.note | map: 'tags' | uniq %}
{{tags}}

<ul>
  {% for tags in page.tags %}
    <li>{{ tags }}</li>
  {% endfor %}
</ul>