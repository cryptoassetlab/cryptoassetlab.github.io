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
{% if post.author %}|* {{ post.author }}*
{% endif %}

{% if post.subtitle %}
<h4>{{ post.subtitle }}</h4>
{% endif %}

{{ post.excerpt }}

<a href="{{ site.baseurl }}{{ post.url }}">Read more</a>
  
{% endfor %}
