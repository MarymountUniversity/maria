---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

MARIA is a mix of full-time faculty, doctoral researchers, and undergraduates.
If you're interested in joining, [reach out](contact).

{% include section.html %}

## Faculty

<div class="team-group">
{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}
</div>

## Doctoral researchers

<div class="team-group">
{% include list.html data="members" component="portrait" filter="role == 'dsc'" %}
</div>

## Undergraduate researchers

<div class="team-group">
{% include list.html data="members" component="portrait" filter="role == 'undergrad'" %}
</div>
