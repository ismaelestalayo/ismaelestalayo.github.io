---
layout: page
permalink: /blog/
title: Blog
description: Tech related posts.
visible: true
---

<ul class="post-list">
	{% for post in site.blog reversed %}
	{% if post.visible == true  %}
	<li>
		<a class="post-list-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
		<p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
		<p class="post-meta">———</p>
	</li>
	{% endif  %}
	{% endfor %}
</ul>