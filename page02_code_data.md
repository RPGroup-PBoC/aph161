---
layout: page
title: Code and Data
img: datum.png # Add image post (optional)
permalink: code
sidebar: true
---

---

{% if site.data.tutorials %}

## Code

{% for tut in site.data.tutorials %}

<article class="post">
<a class="post-thumbnail" style="background-image: url({{site.baseurl}}/{{site.year}}/assets/img/{{tut.pic}})" href="{{site.url}}/{{site.baseurl}}/tutorials/{{tut.link}}.html"> </a>



<div class="post-content">
<b class="post-title"><a href="http://rpgroup.caltech.edu/aph161/assets/tut/{{tut.link}}.html">{{tut.title}}</a></b>
<p> {{tut.desc}}</p>
<p>• <a href="http://rpgroup.caltech.edu/aph161/assets/tut/{{tut.link}}.ipynb"> Jupyter Notebook (.ipynb)</a><br/></p>
{% if fig.req %}<i>Necessary Data Sets </i><br/>
{% for ds in fig.req %}
{% if ds.storage == 'local' %}
{% assign link = "{{site.url}}/{{site.baseurl}}/datasets/{{ds.link}}" %}
{% else %}
{% assign link = "{{ds.link}}" %}
{% endif %}
<a style="font-size: 0.9em;" href="{{link}}"> - {{ds.title}} </a><br/>
{% endfor %}
{% endif %}
</div>

</article>
{%endfor%}
{% endif %}





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



