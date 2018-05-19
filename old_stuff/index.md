---
layout: page
title: Ruminations
tagline: Some thoughts of mine
summary: I decided to start my blog up ... again.
---
{% include JB/setup %}

{% for post in site.posts offset: 0 limit: 10 %}
<div class="row">
  <div class="span7">
    <div class="row">
      <div class="span2">
        <a href="{{ post.url }}" >
            <img border="0" width="250" height="150" src="/img/posts/{{ post.image }}" alt="">
        </a>
      </div>
      <div class="span5">
		<h4><strong><a href="{{ post.url }}">{{ post.title }}</a></strong></h4>
        <p>
          {{ post.summary }}
        </p>
		<p>
          <i class="icon-calendar"></i> {{ post.date | date: "%B %e, %Y" }}
        </p>
        <p><a href="{{ post.url }}">Read more</a></p>
      </div>
    </div>
	<hr>
  </div>
</div>
{% endfor %}

## To-Do

Fix a crapton of stuff!!!
