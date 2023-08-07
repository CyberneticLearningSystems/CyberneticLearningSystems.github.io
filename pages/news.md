---
layout: default
title: News
description: Our latest news and blog posts
---

<div class="content">
	<div class="blog">

		<div class="posts">
			{% assign sorted_posts = site.posts | sort: "modified" | reverse %}
		  {% for post in sorted_posts %}
		    <article class="post">
					<div class="date">
	    			{% assign date_modified = post.modified | date: '%B %d, %Y' %}
	    			{% assign date_created = post.date | date: '%B %d, %Y' %}
	    			{% if date_modified != date_created %}
	    			  Updated {{ date_modified }} (created: {{ date_created }})
	    			{% else %}
	    				Created {{ date_created }}
	    			{% endif %}
					</div>

		      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.post_title }}</a></h1>

		      <div class="entry">
		        {{ post.excerpt }}
		      </div>

		      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
		      
		      <div class="category">
		      	{% if post.category %}
		      		<font size="2" color="grey">Category: {{ post.category }}</font>
						{% endif %}
		      </div>
			  <hr size="2">
		    </article>
		  {% endfor %}
		</div>

	</div>
</div>