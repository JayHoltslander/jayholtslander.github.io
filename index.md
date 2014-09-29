---
layout: page
title: Jay's Jekyll Blog
tagline: With Bootstrap 3!
---
{% include JB/setup %}

<div class="row">
  <div class="col-md-12">
    <div class="jumbotron">
      <p>This is a Jumbotron!</p>
      <a href="#" class="btn btn-lg btn-primary">Hells yeah!</a> 
    </div>
  </div>
</div>

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

{% highlight html %}
<h1>This is an example code block!<h1>
<p>It's not actually rendered as html</p>
{% endhighlight %}


<h3>Recent posts</h3>

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> {{ post.excerpt }}</li>
  {% endfor %}
</ul>


