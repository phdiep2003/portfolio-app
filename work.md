---
layout: default
title: "Work Experience"
---

<h2>Work Experience</h2>
{% for job in site.data.profile.work_history %}
    <h3>{{ job.company }} ({{ job.date }})</h3>
    <p><b>Position:</b> {{ job.position }}</p>
    <p><b>Location:</b> {{ job.location }}</p>
    <ul>
        {% for responsibility in job.responsibilities %}
            <li>{{ responsibility }}</li>
        {% endfor %}
    </ul>
{% endfor %}
