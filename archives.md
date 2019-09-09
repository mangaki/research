---
layout: page
title: Archives
---

{% for post in site.posts %}
<div class="post">
  <h2>
    <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
  </h2>
  <p class="post-meta"><time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%b %-d, %Y" }}</time></p>
  {{ post.excerpt }}
</div>
{% endfor %}
