---
layout: page
title: Team
subtitle: Faculty and students working across physics analysis, detector systems, and computing.
permalink: /team/
nav: team
---
<h2>Faculty</h2>
<div class="team-grid">
{% for item in site.data.faculty %}{% assign person = item[1] %}
<article class="person-card"><a class="avatar" href="{{ '/team/' | append: person.slug | append: '/' | relative_url }}">{{ person.initials }}</a><div><h3><a href="{{ '/team/' | append: person.slug | append: '/' | relative_url }}">{{ person.name }}</a></h3><p class="role">{{ person.role }}</p><p>{{ person.summary }}</p><a class="text-link" href="{{ '/team/' | append: person.slug | append: '/' | relative_url }}">View profile &rarr;</a></div></article>
{% endfor %}
</div>

<h2>Students</h2>
<h3>Current students</h3>
{% if site.data.students.current.size > 0 %}<div class="student-grid">{% for student in site.data.students.current %}<article class="student"><h4>{{ student.name }}</h4><p>{{ student.programme }}{% if student.topic %} - {{ student.topic }}{% endif %}</p><small>{{ student.period }}</small></article>{% endfor %}</div>{% else %}<p class="empty">Student profiles will be added here.</p>{% endif %}

<h3>Previous students</h3>
{% if site.data.students.previous.size > 0 %}<div class="student-grid">{% for student in site.data.students.previous %}<article class="student"><h4>{{ student.name }}</h4><p>{{ student.programme }}{% if student.topic %} - {{ student.topic }}{% endif %}</p><small>{{ student.period }}</small></article>{% endfor %}</div>{% else %}<p class="empty">Alumni profiles will be added here.</p>{% endif %}

