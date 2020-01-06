---
layout: page
title: Syllabus
img: syllabus.png # Add image post (optional)
permalink: syllabus
sidebar: true
---

Note that the syllabus is tentative and subject to change. Check back regularly for the most recent version.

<table>
<tr>
    <th><b>Date</b></th>
    <th><b>Week  </b></th>
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