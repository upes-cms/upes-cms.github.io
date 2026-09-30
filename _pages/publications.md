---
layout: page
title: Publications
subtitle: Selected direct contributions from UPES-CMS members.
permalink: /publications/
nav: publications
---
{% for item in site.data.faculty %}{% assign person = item[1] %}
{% if person.selected_publications %}<section class="publication-group"><h2>{{ person.name }}</h2><ol class="pub-list">{% for pub in person.selected_publications %}<li>{% if pub.url %}<a href="{{ pub.url }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}<br><span>{{ pub.venue }}</span></li>{% endfor %}</ol>{% if person.inspire %}<p><a class="text-link" href="{{ person.inspire }}">Complete publication record on INSPIRE &rarr;</a></p>{% endif %}</section>{% endif %}
{% endfor %}

