---
title: Potential Projects
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

### Currently unprocessed / potential projects

 - Tai Chi+ADHD / Sleep / Feldenkrais / etc.
 - SFZC meditation app
 - Stress management with Pablo Paredes and John Canny
 - TIER / Mezuri
   - Documentation
 - Embodied Underground
 - Mindful Schools
 - 3D javascript visualization toolkit
 - NOAA Satellite date [currently being
   released](https://data-alliance.noaa.gov/).
