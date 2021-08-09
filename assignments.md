---
layout: page
title: Assignments
---

## Assignments

### Homework

{% assign hwbydue = site.hw | sort: "duedate" %}

{% for homework in hwbydue -%}

| [{{ homework.title }}]({{ homework.url | relative_url }}) | Due: {{ homework.duedate | date_to_string: "ordinal", "US"  }} |
{% endfor %}


{% comment %}
### Papers

{% assign papersbydue = site.papers | sort: "duedate" %}

{% for paper in papersbydue -%}

| [{{ paper.title }}]({{ paper.url | relative_url }}) | Due: {{ paper.duedate | date_to_string: "ordinal", "US"  }} |
{% endfor %}
{% endcomment %}

{% comment %}
### Template

[LaTeX template for homework]({{ "/assets/405505-Homework-template.tex" | relative_url }})
{% endcomment %}
