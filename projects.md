---
title: Projects
layout: page
---
<ul class="post-list list-unstyled">

    {% for proj in site.pages %}
        {{ proj.categories }}
        {% if proj.url contains 'projects/' %}

        <li>
            <h2>
                <a class="post-link"
                    href="{{ proj.url | prepend: site.baseurl }}">
                        {{ proj.title }}
                </a>
            </h2>
            <dl class="dl-horizontal">
                <dt>Topic:</dt>
                <dd>{{ proj.topic }}</dd>

                <dt>Client:</dt>
                <dd>{{ proj.client }}</dd>

                {% if proj.team %}
                <dt>Team:</dt>
                <dd>{{ proj.team }}</dd>
                {% endif %}

                {% if proj.mentor %}
                <dt>Mentor:</dt>
                <dd>{{ proj.mentor }}</dd>
                {% endif %}
            </dl>
        </li>

        {% endif %}
    {% endfor %}
</ul>
