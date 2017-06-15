---
layout: page
title: Writing
permalink: /writing/
---

I've been writing full-time about the arts, politics, the environment, agriculture and business for over six years now. In that time my work has appeared in places like The Irish Times, The Sunday Times, The Wire, Resident Advisor, The Quietus, Ear To The Ground, Business & Finance, The Stinging Fly and The Millions. I've written about everything from avant-garde composition to cooperative cattle marts. Below you'll find a partial list of writing I've done during that time, with links where possible.

I'm always open to ideas and usually up for covering new beats. If you'd like to talk about commissioning something, you can reach me at [imaleney@gmail.com](mailto:imaleney@gmail.com). 

<ul class="link-list">
{% assign sorted = site.data.writing_links | sort: "featured" | reverse %}
{% for link in sorted %}
	<li {% if link.featured %} class="featured-link" {% endif %} >
		<a href="{{ link.href }}" rel="noopener" target="_blank">{{ link.title }}, {{ link.date | date: "%B %Y" }}</a>
		{% if link.featured %} 
			<p>{{ link.description}}</p>
		{% endif %}
	</li>
{% endfor %}
</ul>