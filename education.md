---
layout: default
title: "Education"
---

<h2>Education</h2>
{% for edu in site.data.profile.education %}
    <h3>{{ edu.institution }}</h3>
    <p><b>Degree:</b> {{ edu.degree }}</p>
    <p><b>Concentration:</b> {{ edu.concentration }}</p>
    <p><b>Expected Graduation:</b> {{ edu.expected_graduation }}</p>
    <p><b>Certificates:</b> {{ edu.certificates | join: ', ' }}</p>
{% endfor %}
