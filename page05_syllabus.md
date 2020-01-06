---
layout: page
title: Syllabus
img: lab.png # Add image post (optional)
permalink: syllabus
sidebar: true
---

<table>
<tr>
    <th><b>Date</b></th>
    <th><b>Week</b></th>
    <th><b>Topic</b></th>
</tr>
{% for day in site.data.syllabus %}
<tr>
    <td>{{day.date}}</td>
    <td>{{day.week}}</td>
    <td>{{day.topic}}</td>
</tr>
{% endfor %}
</table>

