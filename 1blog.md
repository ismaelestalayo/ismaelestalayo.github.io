---
layout: page
permalink: /blog/
title: Blog
visible: true
description: 
---

<ul class="post-list">
{% for post in site.blog reversed %}
{% if post.visible == true  %}
    <li>
        <h2><a class="post-list-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endif  %}
{% endfor %}
</ul>