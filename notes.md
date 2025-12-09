---
layout: page
title: Notes
---

Praesent pretium metus blandit quam egestas congue. Aenean at efficitur magna. Curabitur bibendum ligula et ligula ornare finibus. Duis placerat, augue in convallis finibus, felis nisl venenatis libero, a rhoncus diam nunc nec quam. Maecenas sed turpis at nisl rhoncus tincidunt. Aliquam lobortis odio et tellus tincidunt luctus. Nulla congue felis vel ex viverra, eget semper nulla condimentum. Sed eu ultricies arcu, eu mollis ante.


{% for article in site.notes %}
	* [{{ article.title }}]({{ site.baseurl }}{{ article.url }})
{% endfor %}




<ol>
{% for article in site.notes %}
<li>
  <a href="{{ site.baseurl }}{{ article.url }}">{{ article.title }}</a>
</li>
{% endfor %}
</ol>
