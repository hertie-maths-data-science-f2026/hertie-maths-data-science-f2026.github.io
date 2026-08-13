---
layout: page
title: Materials
permalink: /materials/
---

Readings by week (lecture slides are on the [Lectures](/lectures/) tab). Released materials
are visible to enrolled students.

{% assign lectures_sorted = site.lectures | sort: 'date' %}
{% for lecture in lectures_sorted %}
{% capture readings %}{% for link in lecture.links %}{% if link.name contains "reading -" %}<li><a href="{% if link.url contains '://' %}{{ link.url }}{% else %}{{ link.url | prepend: site.baseurl }}{% endif %}">{{ link.name | remove: "reading - " }}</a></li>{% endif %}{% endfor %}{% endcapture %}
{% if readings != "" %}
<h3>{{ lecture.title }}</h3>
<ul>{{ readings }}</ul>
{% endif %}
{% endfor %}
