---
layout: default
title:  Neighborhood News and Features
---

# Neighborhood News and Features

<ul class="posts">  
	{% for post in site.posts limit:20 %}  
	   <li>  
		   <span>{{ post.date | date_to_string }}</span> &raquo;  
		   <a href="{{ BASE_PATH }}{{ post.url }}">  
		   {{ post.title }}</a> 
		   {{ post.excerpt }} 
	   </li>  
	{% endfor %}  
</ul>

[View All Posts]({{site.baseurl}}/allnews.html)