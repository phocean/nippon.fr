---
weight: 500
entry: English
layout: page
title: English
---

<ul>
    {% for post in site.categories.english %}
        {% if post.title != null %}
        <li>
            <i>{{ post.date | date: "%Y/%m/%d" }}</i>
            <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
        </li>
        {% endif %}
    {% endfor %}
</ul>

