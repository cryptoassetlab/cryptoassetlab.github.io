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
    <p>
        {{ page.date | date: "%b %e, %Y" }}
        {% if page.author %}
        |<i> {{ page.author }}</i>
        {% endif %}
    </p>

    {% if post.subtitle %}
        <p>{{ post.subtitle }}</p>
    {% endif %}

    <p>{{ post.excerpt }}</p>

    <p><a href="{{ site.baseurl }}{{ post.url }}">Read more</a></p>
  
{% endfor %}
