---
layout: page
title: Jay's Jekyll Blog Project
tagline: with Bootstrap 3!
---
{% include JB/setup %}









### [1 Post post tagged "Featured"]({{ site.url }}/tag-jay/)

<section class="edge-to-edge">

{% for post in site.tags.featured limit:1 %}
  <div class="col-xs-12">
    <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.excerpt }}</a>
  </div>
{% endfor %}

</section>





<h2>Other post requests</h2>


### [4 Posts (max.) from Category A]({{ site.url }}/category-a/)
<section class="edge-to-edge">
<div class="row">
{% for post in site.categories.categorya limit:4 %}
  <div class="col-md-3 col-xs-6">
    <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.excerpt }}</a>
  </div>
{% endfor %}
</div>
</section>




### [3 Posts (max.) from Category B]({{ site.url }}/category-b/)

<div class="row">
{% for post in site.categories.categoryb limit:3 %}
  <div class="col-md-4 col-xs-4">
    <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.excerpt }}</a>
  </div>
{% endfor %}
</div>




### [2 Posts (max.) of posts tagged "Jay"]({{ site.url }}/tag-jay/)

<div class="row">
{% for post in site.tags.jay limit:2 %}
  <div class="col-xs-12 col-md-6">
    <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.excerpt }}</a>
  </div>
{% endfor %}
</div>




### [All posts in all categories]({{ site.url }}/blog)

<div class="row">
  {% for post in site.posts %}
    <div class="col-md-4 col-xs-6">

      <!-- IMAGE -->
        <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.excerpt }}</a>
        <!-- <a href="{{ BASE_PATH }}{{ post.url }}"><img src="{{ post.icon-image }}"></a> -->
      <!-- /IMAGE -->

      <span><a href="{{ BASE_PATH }}{{ post.url }}"><strong>{{ post.title }}</strong></a> Posted on: {{ post.date | date_to_string }}</span>

    </div>
  {% endfor %}
</div>