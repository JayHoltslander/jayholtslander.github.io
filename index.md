---
layout: page
title: Jay's Jekyll Blog Project
tagline: with Bootstrap 3!
---
{% include JB/setup %}


<div class="row">
  <div class="col-md-12">
    <div class="jumbotron">
      <p>Read the Jekyll Bootstrap API</p>
      <a href="http://jekyllbootstrap.com/api/bootstrap-api.html" class="btn btn-lg btn-primary">Continue</a> 
    </div>
  </div>
</div>



{% highlight html %}
<h1>This is an example code block!<h1>
<p>It's not actually rendered as html</p>
{% endhighlight %}


<h3>Recent posts</h3>

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