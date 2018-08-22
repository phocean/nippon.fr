---
layout: page
weigth: 100
entry: Home
title: パリ英語家庭教師
description: フランス、パリ/ブローニュで探す英語家庭教師。子供から大人までの英語レッスン：英文法、英会話、英語エッセイ、資格試験（英検/TOEFL/IB/SAT/IELTS/TOEIC)
permalink: index.html
---

{% for post in site.posts %}

<article class='post'>
  <h1 class='post-title'>
    <a href="{{ site.baseurl }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h1>
  <div class="post-date">{{ post.date | date: "%b %-d, %Y" }}</div>
  {{ post.content }}
</article>

{% endfor %}
