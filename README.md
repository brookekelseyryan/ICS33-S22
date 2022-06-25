---
layout: home
title: 'ICS 33: Intermediate Programming'
nav_exclude: true
permalink: index.html
seo:
  type: Course
  name: 'ICS 33: Intermediate Programming, Summer 2022'
---
# ICS 33: Intermediate Programming

{% assign instructors = site.staffers | where: 'role', 'course' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

## Catalogue description
Introduces Python syntax and semantics for fundamental programming concepts. Constructing programs for varied problems and environments. Using library modules for applications such as graphics, sound, GUI, database, Web, and network programming. Accelerated course for students with previous programming background.

{% if site.announcements.size != 0 %}
## Announcements

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}

{% endif %}
