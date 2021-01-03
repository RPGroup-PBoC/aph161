---
layout: page
title: Homework
img: hw.png # Add image post (optional)
permalink: homework
sidebar: true
---

---

Homeworks are due at the beginning of class one week after they are posted.  Solutions will be posted two days after the homeworks are submitted, and homeworks will be returned a week after they are submitted.

Late policy: NO late homeworks will be accepted (late means anytime after class starts the day the homework is due) unless you have a mindblowingly good excuse - this means a note from someone like a doctor or a Dean.  Rob does not grant extensions.

Collaboration policy: you may discuss the homework with others, but your explanations and derivations must be your own.  Your logic and the *significance* of your results should also be explained.

<table>
<tr>
<th> <b>Homework</b></th>
<th> <b> Due Date</b> </th>
<th> <b> Solutions</b> </th><br/>
</tr>
{% for hwk in site.data.homework %}
<tr>
<td> <a href="assets/hwk/{{hwk.pset}}"> {{hwk.name}} </a></td>
<td> {{hwk.due_date}} </td> 
{% if hwk.solns %}
<td>
  <a href="http://rpdata.caltech.edu/courses/aph161/protected/{{site.year}}/solutions/{{hwk.solns}}"><b class="post-title">{{'Solutions'}}</b></a> 
  {% if hwk.code_files %}
    <br/>
      <a href="http://rpdata.caltech.edu/courses/aph161/protected/{{site.year}}/solutions/{{hwk.code_files}}"><b class="post-title">{{'Code files (.zip)'}}</b></a>
  {% endif  %}
</td>
{% else %}  
   <td> {{'-'}} </td>
  {% endif %}
  </tr>
  {%endfor%}
</table>

  


