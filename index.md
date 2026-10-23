
---
layout: default
title: Home
---

# Things worth remembering

This is my personal developer knowledge base.

## Jekyll test

Site title: {{ site.title }}

Number of posts: {{ site.posts.size }}

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

{% if site.posts.size == 0 %}
No posts published yet.
{% endif %}
