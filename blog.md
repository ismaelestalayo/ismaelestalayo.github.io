---
layout: page
permalink: /blog/
title: Blog
description: Thoughts, tutorials, discussions...
---

<ul class="post-list">
{% for post in site.blog reversed %}
{% if post.visible == true  %}
    <li>
        <h2><a class="poem-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endif  %}
{% endfor %}
</ul>