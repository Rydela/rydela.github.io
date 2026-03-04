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
    {% assign badge_label = link.badge_label | default: link.label %}
    {% assign badge_message = link.badge_message | default: 'Open' %}
    {% assign label_slug = badge_label | replace: ' ', '_' %}
    {% assign message_slug = badge_message | replace: ' ', '_' %}
    {% assign logo = 'Link' %}
    {% if link.logo %}
      {% assign logo = link.logo %}
    {% elsif link.label == 'GitHub' or link.label == 'Repository' %}
      {% assign logo = 'GitHub' %}
    {% elsif link.label == 'Live Project' %}
      {% assign logo = 'Google-Chrome' %}
    {% elsif link.label == 'Article' %}
      {% assign logo = 'Medium' %}
    {% elsif link.label == 'Organization' %}
      {% assign logo = 'OpenCollective' %}
    {% endif %}
    {% assign badge_color = link.badge_color | default: '2b6cb0' %}
    <a href="{{ link.url }}">
      <img alt="{{ link.label }}" src="https://img.shields.io/badge/{{ label_slug }}-{{ message_slug }}-{{ badge_color }}?logo={{ logo }}">
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
