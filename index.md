---
layout: default
permalink: /
title: Your Site Title
description: Your description
---

# Home?

# Latest Posts

{% for post in site.posts limit:3 %}
## [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

[Read more...]({{ post.url }})

---
{% endfor %}

# Posts Debug

Number of posts: {{ site.posts.size }}

{% if site.posts.size > 0 %}
Posts found:
{% for post in site.posts %}
- {{ post.title }} ({{ post.date }})
{% endfor %}
{% else %}
No posts found!
{% endif %}
