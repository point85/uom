---
layout: page
title: Blog
description: Blog for posts related to units of measure.
permalink: /blog/
---

{% for post in site.posts %}
  <article class="post">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h2>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
    {{ post.excerpt }}
  </article>
{% endfor %}
