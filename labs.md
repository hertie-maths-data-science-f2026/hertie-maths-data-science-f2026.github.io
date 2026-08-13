---
layout: page
title: Labs
permalink: /labs/
---

Lab exercises by week (lecture slides are on the [Lectures](/lectures/) tab). Released
materials are visible to enrolled students.

{% assign lectures_sorted = site.lectures | sort: 'date' %}
{% for lecture in lectures_sorted %}
{% capture labs %}{% for link in lecture.links %}{% if link.name contains "lab -" %}<li><a href="{% if link.url contains '://' %}{{ link.url }}{% else %}{{ link.url | prepend: site.baseurl }}{% endif %}">{{ link.name | remove: "lab - " }}</a></li>{% endif %}{% endfor %}{% endcapture %}
{% if labs != "" %}
<h3>{{ lecture.title }}</h3>
<ul>{{ labs }}</ul>
{% endif %}
{% endfor %}
