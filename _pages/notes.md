---
title: "All My Notes"
permalink: /notes/
---

<ul>
    {% for note in site.pages %}
        <li>
            <a href="{{site.baseurl}}{{note.url}}">{{note.title}}</a>
        </li>
    {% endfor %}
</ul>
