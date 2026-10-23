---
layout: default
title: Home
---

# Things worth remembering.

A collection of development notes, experiments,
and occasional deep dives into software engineering.

Mostly things I've learned, built, broken, or
figured out along the way.

This is my personal knowledge base, made public
in case someone else finds it useful.

---

[All]({{ "/" | relative_url }}) ·
[Posts]({{ "/posts/" | relative_url }}) ·
[Notes]({{ "/notes/" | relative_url }}) ·
[Tags]({{ "/tags/" | relative_url }})

---

## Latest entries

{% for post in site.posts %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.kind | capitalize }}**
· {{ post.date | date: "%B %d, %Y" }}

{% if post.description %}
{{ post.description }}
{% endif %}

{% for tag in post.tags %}
`#{{ tag }}`
{% endfor %}

---

{% endfor %}
