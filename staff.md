---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff 🍎

To help us quickly identify course-related emails and respond to you, please try using the format: ICS33: First Name Last Name – Subject. Please ensure to include both the instructor (lu.he@uci.edu) and the TA (brooke.ryan@uci.edu) in the email.

## Instructor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistant

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
