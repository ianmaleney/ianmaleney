---
layout: page
title: Writing
permalink: /writing/
---

My writing has appeared in places like The Irish Times, The Sunday Times, The Wire, Resident Advisor, The Quietus, Music & Literature, The Stinging Fly and The Millions. I've written about everything from avant-garde composition to cooperative cattle marts. Below you'll find a partial list of my work, beginning with the most recent, including links where possible.

If you'd like to talk about commissioning something, you can reach me at [imaleney@gmail.com](mailto:imaleney@gmail.com). 

<ul class="link-list">
{% assign sorted = site.data.writing_links | reverse %}
{% for link in sorted %}
	<li {% if link.featured %} class="featured-link" {% endif %} >
		<a href="{{ link.href }}" rel="noopener" target="_blank">{{ link.title }}, {{ link.date | date: "%B %Y" }}</a>
		{% if link.featured %} 
			<p>{{ link.description}}</p>
		{% endif %}
	</li>
{% endfor %}
</ul>