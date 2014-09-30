---
layout: page
title: "Category B"
description: ""
---
{% include JB/setup %}

<p>This is Category B page</p>

### [All Posts from Category B]({{ site.url }}/category-b/)

<ul class="th-grid-full">
{% for post in site.categories.categoryb %}
  <li><a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}"><img src="{{ site.url }}/images/{{ post.image.thumb }}" alt="thumbnail image"></a></li>
{% endfor %}
</ul>
