---
layout: index-list
title: Writing
permalink: /writing/
---

My writing has appeared in places like the _Irish Times_, the _Sunday Times_, _The Wire_, _Resident Advisor_, _The Quietus_, _Music & Literature_, _The Stinging Fly_ and _The Millions_. I've written about everything from avant-garde composition to cooperative cattle marts. Below you'll find a partial list of my work, beginning with the most recent, including links where possible.

If you'd like to talk about commissioning something, you can reach me at [imaleney@gmail.com](mailto:imaleney@gmail.com). 

<ul class="link-list">
{% assign sorted = site.data.writing_links | reverse %}
{% for link in sorted %}
	<li {% if link.featured %} class="featured-link" {% endif %} >
		<a href="{{ link.href }}" rel="noopener" target="_blank">{{ link.title }}, {{ link.date | date: "%B %Y" }}</a>
		<!--{% if link.featured %} 
			<p>{{ link.description}}</p>
		{% endif %}-->
	</li>
{% endfor %}
</ul>