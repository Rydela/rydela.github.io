---
layout: default
---

# Portfolio

{% assign all_projects = site.projects | sort: "year" | reverse %}
Most recent work first.

{% for project in all_projects %}
### [{{ project.title }}]({{ project.url | relative_url }})

**{{ project.year }}** · {{ project.status | capitalize }}

<p>
  {% for link in project.links %}
    {% assign label_slug = link.label | replace: ' ', '_' %}
    {% assign logo = 'Link' %}
    {% if link.label == 'GitHub' or link.label == 'Repository' %}
      {% assign logo = 'GitHub' %}
    {% elsif link.label == 'Live Project' %}
      {% assign logo = 'Google-Chrome' %}
    {% elsif link.label == 'Article' %}
      {% assign logo = 'Medium' %}
    {% elsif link.label == 'Organization' %}
      {% assign logo = 'OpenCollective' %}
    {% endif %}
    <a href="{{ link.url }}">
      <img alt="{{ link.label }}" src="https://img.shields.io/badge/{{ label_slug }}-Open-2b6cb0?logo={{ logo }}">
    </a>
  {% endfor %}
</p>

<div style="text-align: justify">{{ project.summary }} {{ project.outcome }}</div>
<br>
{% if project.image %}
<center><img src="{{ project.image | relative_url }}" alt="{{ project.title }}"></center>
<br>
{% endif %}
---
{% endfor %}

<center>© {{ "now" | date: "%Y" }} Ryan Arias Delafosse - Data Scientist portfolio.</center>
