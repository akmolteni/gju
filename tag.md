---
layout: page
title: Tag
---

{% include archives.html %}
Browse posts with tags
{% assign sorted_tags = (site.tags | sort:0) %}
{% assign sorted_tags = (site.tags | sort_natural) %}

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

