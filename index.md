---
layout: default
permalink: /
title: Your Site Title
description: Your description
---

# Home?

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[View all posts](/posts/)
