---
layout: page
title: Staff and office hours
description: A listing of all the course staff members.
---

# Staff

## Professor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Course Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign ACE_assistants = site.staffers | where: 'role', 'ACE Assistant' %}
## [ACE](https://engineering.stanford.edu/students-academics/equity-and-inclusion-initiatives/undergraduate-programs/additional-courses) Course Assistant

{% for staffer in ACE_assistants %}
{{ staffer }}
{% endfor %}