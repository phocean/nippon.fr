---
weight: 400
entry: Français
layout: page
title: Français
---

<ul>
    {% for post in site.categories.french %}
        {% if post.title != null %}
        <li>
            <i>{{ post.date | date: "%Y/%m/%d" }}</i>
            <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
        </li>
        {% endif %}
    {% endfor %}
</ul>
