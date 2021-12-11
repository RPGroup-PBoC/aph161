---
layout: page
title: Syllabus
img: syllabus.png # Add image post (optional)
permalink: syllabus
sidebar: true
---



<b>Required text:</b> Physical Biology of the Cell (2nd ed) by Phillips, Kondev, Theriot and Garcia (ISBN: 0815344503)

The syllabus ([PDF](http://rpdata.caltech.edu/courses/aph161/2021/161_2021_syllabus.pdf)) is tentative and subject to change. Refer to the list below for the prerecorded video lectures.



<table>
<tr>
    <th style="width:130px"><b>Date</b></th>
    <th><b>Topic</b></th>
</tr>
{% for day in site.data.syllabus %}
<tr>
    <td>{{day.date}}  </td>
    <td>{{day.topic}}
    {% if day.videos %}
    {% for v in day.videos %}
    {% if v.name %}
    <a href="http://rpdata.caltech.edu/courses/aph161/2021/videos/{{v.name}}">{{v.title}}</a><br/>
    {% else %} 
    <a href="{{v.url}}">{{v.title}}</a><br/>
    {%endif %}
    {%endfor%}
    {%endif %}
    </td> 

  <!-- {% if day.slide %} 
  <td>
  {% for s in day.slide %}
  <a href="http://rpdata.caltech.edu/courses/aph161/protected/2020/videos/{{s}}"><b class="post-title">{{s}}</b></a> 
  {%endfor%}
  </td>
  {% else %}
  <td> {{'-'}} </td>
  {% endif %} -->
</tr>
{% endfor %}
</table>