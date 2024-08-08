---
layout: page
title: Announcements
description: A feed containing all of the class announcements.
---

# Announcements

Course announcements will be posted on Brightspace.

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}


#nav_exclude: true
