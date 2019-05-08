---
title: "News"
layout: newslay
excerpt: "News Page"
permalink: /news/
---

## News

{% for post in site.posts %}

<h3 class="post-title">
    [{{ post.title }}]({{ post.url }})
</h3>
{{ post.date | date: "%b %e, %Y" }}

{{ post.excerpt }}
  
{% endfor %}
