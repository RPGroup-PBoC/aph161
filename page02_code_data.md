---
layout: page
title: Code and Data
img: datum.png # Add image post (optional)
permalink: code
sidebar: true
---

---



{% if site.data.datasets %}

## Data Sets
{% for ds in site.data.datasets %}
* [{{ds.name}}]({%if ds.storage !=
  'remote'%}{{site.baseurl}}/datasets/{{ds.link}}{%
  else%}{{site.link}}{% endif %}) \| {% if ds.filetype %}(filetype:
  {{ds.filetype}}){%endif%}{% if ds.filesize %}({{ds.filesize}}){%endif%}{%
  if ds.storage == remote %} DOI: {{ds.DOI}}{%endif%}
{% endfor %}
{% endif %}



