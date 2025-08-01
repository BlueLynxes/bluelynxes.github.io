---
layout: default
title: "Rabbithole"
description: "Utilizing my Freedom of Speech until we become the new CCP"
---

# Recent Posts

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

---
{% endfor %}

{% if site.posts.size == 0 %}
No posts found yet.
{% endif %}
