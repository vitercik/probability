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
