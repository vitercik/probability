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

## Course Assistants

{% assign course_assistants = site.staffers | where: 'role', 'Course Assistant' | sort: 'name' %}
{% for staffer in course_assistants %}
{{ staffer }}
{% endfor %}

## ACE Course Assistant

{% assign ace_assistants = site.staffers | where: 'role', 'ACE Course Assistant' %}
{% for staffer in ace_assistants %}
{{ staffer }}
{% endfor %}
