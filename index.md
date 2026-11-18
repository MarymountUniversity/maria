---
---

# Applied AI research at <span class="gradient-text">Marymount</span>

{% capture lead %}
MARIA brings faculty, doctoral, graduate, and undergraduate researchers together to apply
machine learning, natural language processing, and data science to real problems in
health care, cybersecurity, education, and beyond, with an emphasis on mentorship,
collaboration across schools, and open, reproducible research.
{% endcapture %}
<p class="lead">{{ lead | strip }}</p>

{% assign members = site.members | size %}
{% assign theses = site.data.theses | size %}
{% assign current = site.data.doctoral_students | size %}

<div class="stats">
  <div><span class="stat-number gradient-text">{{ site.data.citations | size }}</span><span class="stat-label">Publications</span></div>
  <div><span class="stat-number gradient-text">{{ theses }}</span><span class="stat-label">Doctoral theses advised</span></div>
  <div><span class="stat-number gradient-text">{{ current }}</span><span class="stat-label">Current doctoral students</span></div>
  <div><span class="stat-number gradient-text">{{ members }}</span><span class="stat-label">Lab members</span></div>
</div>

{% include section.html %}

## Research areas

<div class="areas">
{% include area-card.html icon="fa-solid fa-language" title="Natural Language Processing" text="Sentiment analysis, topic modeling, and parsing, with a focus on under-resourced languages including Czech, Indonesian, Tamil, Icelandic, and Nepali." link='research/?search="tag: nlp"' %}
{% include area-card.html icon="fa-solid fa-shield-halved" title="AI for Cybersecurity" text="Deepfake detection, identity and access management, open cybersecurity datasets, and synthetic data for doctoral research." link='research/?search="tag: cybersecurity"' %}
{% include area-card.html icon="fa-solid fa-heart-pulse" title="Health AI" text="Privacy-preserving gait analysis with synthetic video (NIH AIM-AHEAD) and human-in-the-loop prediction for falls prevention." link='research/?search="tag: health"' %}
{% include area-card.html icon="fa-solid fa-vr-cardboard" title="HCI, Robots & XR" text="Persuasive communication in human–robot interaction, LLM-assisted communication in the metaverse, and VR for teaching." link='research/?search="tag: hci"' %}
{% include area-card.html icon="fa-solid fa-chart-line" title="Applied Data Science" text="Machine learning for juvenile justice, misinformation, business strategy, and other problems brought by partners across campus." link='research/?search="tag: data-science"' %}
{% include area-card.html icon="fa-solid fa-chalkboard" title="AI in Education" text="Using NLP to inform curricula, analyze student needs, and map research trends in computing and doctoral programs." link='research/?search="tag: education"' %}
</div>

{% include section.html %}

## Latest publications

{% assign latest = site.data.citations | sort: "date" | reverse %}
{% for citation in latest limit: 4 %}
  {% include citation.html
    id=citation.id
    title=citation.title
    authors=citation.authors
    publisher=citation.publisher
    date=citation.date
    link=citation.link
    type=citation.type
    tags=citation.tags
  %}
{% endfor %}

{%
  include button.html
  link="research"
  text="All publications"
  icon="fa-solid fa-arrow-right"
  flip=true
%}

{% include section.html %}

## Get involved

<div class="areas">
{% include area-card.html icon="fa-solid fa-graduation-cap" title="Doctoral research" text="Current D.Sc. students and the theses our faculty have advised." link="doctoral" cta="Browse theses" %}
{% include area-card.html icon="fa-solid fa-users" title="Our team" text="Faculty, doctoral researchers, and undergraduates working across disciplines." link="team" cta="Meet the team" %}
{% include area-card.html icon="fa-solid fa-envelope" title="Join the lab" text="Students at any level with a research idea, or faculty looking for an AI collaborator, are welcome." link="contact" cta="Get in touch" %}
</div>
