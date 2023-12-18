---
layout: default
title: Reviews
---
# Recent Reviews

<ul>
    {% for post in site.categories.reviews %}
        {% if post.url %}
            <li>
                <p><a href="{{ post.url }}">{{ post.title }}</a> &#8212; {{ post.date | date_to_long_string }}</p>
                {{ post.excerpt }}
            </li>
        {% endif %}
    {% endfor %}
</ul>
