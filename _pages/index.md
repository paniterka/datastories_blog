--- 
title: Welcome!
permalink: /
author_profile: true 

---
<div class="welcome">
Hello! Welcome to my blog. There is content in English and in Polish. Enjoy! 
</div>

<div class="latest_in">
	<h1>Latest in English...</h1>
	<div class="grid__wrapper">
	  {% assign collection = 'en' %}
	  {% assign posts = site[collection] | reverse %}
	  {% for post in posts limit:1%}
		{% include archive-single.html type="list" %}
	  {% endfor %}
	</div>
</div>

<div class="latest_in">
	<h1>Najnowsze po polsku...</h1>
	<div class="grid__wrapper">
	  {% assign collection = 'pl' %}
	  {% assign posts = site[collection] | reverse %}
	  {% for post in posts limit:1%}
		{% include archive-single.html type="list" %}
	  {% endfor %}
	</div>
</div>

