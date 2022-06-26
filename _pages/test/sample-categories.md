---
title: "Categories"
permalink: /categories-sample/
---

<ul>
    {% for note in site.pages %}
        {% if note.categories %}
        {{ note.title }}
        <li>
            {{ note.categories }}
        </li>
        {% endif %}
    {% endfor %}
</ul>


<ul>
    {% for category in site.categories %}
        <li>
            {{ category.url }} {{ category.link }} {{ category.title }}
        </li>
    {% endfor %}
</ul>
