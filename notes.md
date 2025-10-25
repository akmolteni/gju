---
layout: page
title: Notes
---

<p>
	Notes are just notes.
</p>

<ol>
{% for article in site.notes %}
<li>
  <a href="{{ site.baseurl }}{{ article.url }}">{{ article.title }}</a>
</li>
{% endfor %}
</ol>
