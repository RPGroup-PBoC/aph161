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
</tr>
{% for day in site.data.syllabus %}
<tr>
    <td>{{day.date}}  </td>
    <td>{{day.week}}  </td>
    <td>{{day.topic}}<br/>
    {% if day.videos %}
    {% for v in day.videos %}
    <a href="http://rpdata.caltech.edu/courses/aph161/2021/videos/{{v.name}}">{{v.title}}</a><br/>
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