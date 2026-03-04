---
layout: default
title: Portfolio
permalink: /portfolio/
---

# Portfolio Index

{% assign all_projects = site.projects | sort: "year" | reverse %}
Most recent work first.

<table>
  <thead>
    <tr>
      <th>Year</th>
      <th>Project</th>
      <th>Status</th>
      <th>Primary Link</th>
    </tr>
  </thead>
  <tbody>
    {% for project in all_projects %}
    {% assign primary = project.links | first %}
    <tr>
      <td>{{ project.year }}</td>
      <td><a href="{{ project.url | relative_url }}">{{ project.title }}</a></td>
      <td>{{ project.status | capitalize }}</td>
      <td><a href="{{ primary.url }}">{{ primary.label }}</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>
