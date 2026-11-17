---
title: Doctoral
nav:
  order: 3
  tooltip: Doctoral students and theses
---

# {% include icon.html icon="fa-solid fa-graduation-cap" %}Doctoral Research

MARIA mentors doctoral students in Marymount's D.Sc. in Cybersecurity program, with dissertations applying AI and machine learning to security, privacy, and trust.

{% include section.html %}

## Current Doctoral Students ({{ site.data.doctoral_students | size }})

{% include list-by-advisor.html component="student-card" data="doctoral_students" %}

{% include section.html %}

## Completed Dissertations ({{ site.data.theses | size }})

{% include list-by-advisor.html component="thesis-card" data="theses" %}
