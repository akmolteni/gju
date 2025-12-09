---
layout: page
title: Notes
---

<p>
	By treating our notes as living documents, I capture the most current, relevant thinking.
	This approach doesn’t replace formal reviews but makes my mental models more effective by keeping them in sync with reality. 
	It forces me to make a decision, challenge my own assumptions, test ideas, and continuously improve my understanding.
</p>
<p>
	I may be inventing the wheel. That's the point. It’s a process of starting from scratch and stripping away assumptions 
	or preconceived notions, in order to understand the core of how things work.
</p>

<ol>
{% for article in site.notes %}
<li>
  <a href="{{ site.baseurl }}{{ article.url }}">{{ article.title }}</a>
</li>
{% endfor %}
</ol>
