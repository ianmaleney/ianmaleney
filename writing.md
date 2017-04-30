---
layout: page
title: Writing
permalink: /writing/
---
<ul class="link-list">
{% for link in site.data.links %}
	<li><a href="{{ link.href }}" rel="noopener" target="_blank">{{ link.title }} | {{ link.location }} </a></li>
{% endfor %}
</ul>