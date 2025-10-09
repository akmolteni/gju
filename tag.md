---
layout: default
title: Tag
---

# Tag
{% assign sorted_tags = (site.tags | sort:0) %}

The Tags:
{% for tag in sorted_tags %}
{% assign all_tags = all_tags | append: tag | append: "," %}
{% endfor %}
{{all_tags}}
---

All tags: 
{% for tag in sorted_tags %}{{ tag[0] }}, {% endfor %}

Browse all posts by tag
{% for tag in sorted_tags %}
  <h2>{{ tag[0] }}</h2>
  <ul>
    {% for post in tag[1] %}
       <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
       			<span>{{ post.date | date_to_string }}</span><!--<span>{{ post.category }}</span>-->
    </li>
    {% endfor %}
  </ul>
{% endfor %}

