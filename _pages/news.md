---
title: "News"
layout: textlay
excerpt: "News Page"
permalink: /news/
---

## News

{% for post in site.posts %}

<h1 class="post-title">
    [{{ post.title }}]({{ post.url }})
</h1>
{{ post.date | date: "%b %e, %Y" }}

{{ post.excerpt }}
  
{% endfor %}
