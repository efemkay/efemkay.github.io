---
title: "All My Notes"
permalink: /notes/
---

<ul>
    {% for note in site.pages %}
        {% if note.categories %}
        <li>
            <a href="{{site.baseurl}}{{note.url}}">{{note.title}}</a>
        </li>
        {% endif %}
    {% endfor %}
</ul>
