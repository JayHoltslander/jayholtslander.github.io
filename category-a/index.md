---
layout: page
title: "Category A"
description: ""
---
{% include JB/setup %}

<p>This is Category A page</p>

### [All Posts from Category A]({{ site.url }}/category-b/)

<ul class="th-grid-full">
{% for post in site.categories.categorya %}
  <li><a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}"><img src="{{ site.url }}/images/{{ post.image.thumb }}" alt="thumbnail image"></a></li>
{% endfor %}
</ul>
