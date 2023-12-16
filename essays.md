---
layout: default
title: Essays
---
# Recent Essays

<ul>
    {% for post in site.categories.essays %}
        {% if post.url %}
            <li>
                <p><a href="{{ post.url }}">{{ post.title }}</a></p>
                {{ post.excerpt }}
            </li>
        {% endif %}
    {% endfor %}
</ul>
