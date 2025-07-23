---
title: Doctoral
nav:
  order: 2
  tooltip: Email, address, and location
---


<h2>Loaded Student Data:</h2>
<pre>{{ site.data.doctoral_students | jsonify }}</pre>


## Current Doctoral Students

{% include list-by-advisor.html component="student-card" data="doctoral_students" %}

---

##  Completed Theses

{% include list-by-advisor.html component="thesis-card" data="theses" %}