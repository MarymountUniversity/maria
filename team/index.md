---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

If you are interested in joining, please reach out to a member of our team.

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}
{% include list.html data="members" component="portrait" filter="role != 'principal-investigator'" %}

{% include section.html background="images/background.jpg" dark=true %}


{% include section.html %}

{% capture content %}

{% endcapture %}

{% include grid.html style="square" content=content %}
