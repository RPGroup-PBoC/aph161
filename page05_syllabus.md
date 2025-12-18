---
layout: page
title: Syllabus
img: syllabus.png # Add image post (optional)
permalink: syllabus
sidebar: true
---



<b>Required text:</b> Physical Biology of the Cell (2nd ed) by Phillips, Kondev, Theriot and Garcia (ISBN: 0815344503)

The syllabus is tentative and subject to change. Refer to the list below for the prerecorded video lectures, which you can find at 
<a href="https://www.youtube.com/@physicalbiologyofthecellca307/videos" target="_blank">
the Physical Biology of the Cell YouTube channel
</a>.



<table>
<tr>
    <th style="width:130px"><b>Date</b></th>
    <th><b>Topic</b></th>
</tr>
{% for day in site.data.syllabus %}
<tr>
  <td>{{day.date}}  </td>
  <td>{% for t in day.topics%}
      <b>{{t.title}}</b><br>
      {% if t.description %}
      {{t.description}}<br>
      {% endif %}
    {%endfor%}
  </td>
</tr>
{%endfor%}
</table>