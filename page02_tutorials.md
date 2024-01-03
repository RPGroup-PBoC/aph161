---
layout: page
title: Tutorials
img: datum.png # Add image post (optional)
permalink: tutorials
sidebar: true
---

---
During this course, you will develop a computational prowess that will aid in your understanding of physical biology. These will be done using Jupyter notebooks through Google Colab, so you will need to sign into a Google Account to create new notebooks.

We will post links to Jupyter Notebooks hosted on Colab of the tutorial sessions here.

{% if site.data.tutorials %}

{% for tut in site.data.tutorials %}

<article class="post">
<a class="post-thumbnail" style="background-image: url({{site.url}}/{{site.baseurl}}/assets/img/{{tut.pic}})" href="{{tut.link}}" target="_blank"> </a>



<div class="post-content">
<b class="post-title"><a href="{{tut.link}}">{{tut.title}}</a></b>
<p> {{tut.desc}}</p>
<p>• <a href="{{tut.link}}" target="_blank"> Google Colab</a><br/></p>
{% if fig.req %}<i>Necessary Data Sets </i><br/>
{% for ds in fig.req %}
<a style="font-size: 0.9em;" href="{{tut.link}}"> - {{ds.title}} </a><br/>
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



