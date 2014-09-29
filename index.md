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

<h3>iOS App launchers <small>(Not for Desktop use)</small></h3>
<a href="tel:+17783840424" class="btn btn-success"><i class="fa fa-phone"></i> Call</a>
<a href="facetime://j.holtslander@gmail.com" class="btn btn-success"><i class="fa fa-video-camera"></i> Facetime</a>
<a href="skype:jason.holtslander?call" class="btn btn-info"><i class="fa fa-skype"></i> Skype</a>
<a href="imessage:j.holtslander@gmail.com" class="btn btn-primary"><i class="fa fa-comment"></i> iMessage</a>

<a href="twitter://user?screen_name=j_holtslander" class="btn btn-default"><i class="fa fa-twitter"></i> Twitter App Link</a>
<a href="instagram://user?username=j_holtslander" class="btn btn-default"><i class="fa fa-instagram"></i> Instagram App Link</a>
<a href="pinterest://user/j_holtslander/" class="btn btn-default"><i class="fa fa-pinterest"></i> Pinterest App Link</a>
<a href="linkedin://#profile/9999" class="btn btn-default"><i class="fa fa-linkedin"></i> Linkedin App Link</a>
<a href="fb://profile/570792107" class="btn btn-default"><i class="fa fa-facebook"></i> Facebook App Link</a>





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