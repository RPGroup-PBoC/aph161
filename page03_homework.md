---
layout: page
title: Homework
img: code.png # Add image post (optional)
permalink: homework
sidebar: true
---

---

<table>
<tr>
<th> <b>Homework</b></th>
<th> <b> Due Date</b> </th>
<th> <b> Solutions</b> </th><br/>
</tr>
{% for hwk in site.data.homework %}
<tr>
<td> <a href="{{site.baseurl}}/assets/hwk/{{hwk.pset}}"> {{hwk.name}} </a></td>
<td> {{hwk.due_date}} </td> 
<td> <a href="https://rpdata.caltech.edu/courses/aph161/2020/{{hwk.solns}}">Solutions</a></td>
</tr>
{%endfor%}
</table>


