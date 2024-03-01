---
layout: page
title: Projects
permalink: /projects/
toggle: on
rank: 1
---

<div class="lab-wrapper">
    <ul class="lab-list">
    {% for project in site._data.projects %}
        <li>
            <h2>{{ project.name }}</h2>
            {% if project.photo %}
                <img class="float-right projects-photo" src="{{ project.photo | prepend: site.images_dir | prepend: site.baseurl }}">
            {% endif %}
            {% if project.collaborators %}
                <p><b>Collaborators: </b>{{ project.collaborators }}</p>
            {% endif %}
        </li>
    {% endfor %}
    </ul>
</div>
