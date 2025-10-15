---
layout: default
title: Category
---

{% include archives.html %}

# Category
{% assign sorted_items = (site.categories | sort:0) %}

All categories: 
{% for item in sorted_items %}{{ item[0] }}, {% endfor %}

Browse all posts by category
{% for item in sorted_items %}
  <h2>{{ item[0] }}</h2>
  <ul>
    {% for post in item[1] %}
       <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
       			<span>{{ post.date | date_to_string }}</span>
    </li>
    {% endfor %}
  </ul>
{% endfor %}
