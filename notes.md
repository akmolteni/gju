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
		<a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
	</li>
{% endfor %}
</ul>

## Title

<ol>
{% for article in site.notes %}
<li>
  <a href="{{ site.baseurl }}{{ article.url }}">{{ article.title }}</a>
</li>
{% endfor %}
</ol>
