---
title: "News"
layout: newslay
excerpt: "News Page"
permalink: /news/
---

## News

{% for post in site.posts %}

### [{{ post.title }}]({{ post.url }})

{{ post.date | date: "%b %e, %Y" }}
{% if post.author %}| *{{ post.author }}*{% endif %}

{% if post.subtitle %}

#### {{ post.subtitle }}

{% endif %}

{{ post.excerpt }}

[Read more]({{ site.baseurl }}{{ post.url }})
  
{% endfor %}
