---
layout: page
title: Archive
permalink: /archive/
---

{% assign ordered_posts = site.posts | sort: "date" | reverse %}
{% for post in ordered_posts %}
- {{ post.date | date: "%B %-d, %Y" }} — [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
