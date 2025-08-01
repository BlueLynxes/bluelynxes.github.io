---
layout: default
permalink: /
title: Your Site Title
description: Your description
---

# Home?

{% for post in site.posts limit:3 %}
## [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

[Read more...]({{ post.url }})

---
{% endfor %}
