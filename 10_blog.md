---
layout: page
weigth: 100
entry: Articles
title: Nippon.fr Blog
description: blog, journal, ブログ, article
permalink: blog.html
---

{% for post in site.posts %}

<article class='post'>
  <h3 class='post-title'>
    <a href="{{ site.baseurl }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h3>
  <div class="post-date">{{ post.date | date: "%b %-d, %Y" }}</div>
  {{ post.content }}
</article>

{% endfor %}
