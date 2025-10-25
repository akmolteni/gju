---
layout: page
title: Notes
---

<p>
	Notes are just notes.
	If the note does not make sense, that's OK.
	I'm trying to make sense of them too.
</p>

{% assign pagesList = site.pages | sort: "category" %}
<ul>
{% for page in pagesList %}
	<li>
		<a href="{{ page.url | absolute_url }}">{{ page.title }}</a>
	</li>
{% endfor %}
</ul>
