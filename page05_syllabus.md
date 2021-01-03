---
layout: page
title: Syllabus
img: syllabus.png # Add image post (optional)
permalink: syllabus
sidebar: true
---



<b>Required text:</b> Physical Biology of the Cell (2nd ed) by Phillips, Kondev, Theriot and Garcia (ISBN: 0815344503)



Note that the syllabus is tentative and subject to change. Check back regularly for the most recent version.

<table>
<tr>
    <th style="width:100px"><b>Date</b></th>
    <th style="width:70px"><b>Week  </b></th>
    <th><b>Topic</b></th>
    <th style="width:70px"><b>Slides</b></th>
</tr>
{% for day in site.data.syllabus %}
<tr>
    <td>{{day.date}}  </td>
    <td>{{day.week}}  </td>
    <td>{{day.topic}}</td>
  {% if day.slide %} 
  <td>
  <a href="http://rpdata.caltech.edu/courses/aph161/protected/{{site.year}}/slides/{{day.slide}}"><b class="post-title">{{'Slides'}}</b></a> </td>
  {% else %}
  <td> {{'-'}} </td>
  {% endif %}
</tr>
{% endfor %}
</table>