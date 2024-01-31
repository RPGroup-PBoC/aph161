---
layout: page
title: Homework
img: hw.png # Add image post (optional)
permalink: homework
sidebar: true
---

---

Homeworks are due 30min before class (2:00 PM) one week after they are posted.  Solutions will be posted two days after the homeworks are submitted, and homeworks will be returned a week after they are submitted.

Late policy: NO late homeworks will be accepted (late means anytime after class starts the day the homework is due) unless you have a mindblowingly good excuse - this means a note from someone like a doctor or a Dean.  Rob does not grant extensions.

Submission policy: Submit all write-ups as PDFs and all Jupyter code as **both** .ipynb and .html files. Your written solutions should be clear and understandable throughout so that we can follow your reasoning. Submit your files for **odd** homeworks to [tom@caltech.edu](mailto:tom@caltech.edu) and for **even** homeworks to [jordan.santana@caltech.edu](mailto:jordan.santana@caltech.edu) with the subject line “HW # - FirstName LastName”.

Collaboration policy: you may discuss the homework with others, but your explanations and derivations must be your own.  Your logic and the *significance* of your results should also be explained.

ChatGPT policy: While we encourage you work on homework problems that involve coding, the use of ChatGPT is allowed for coding parts of homework problems. If you decide to use ChatGPT, we ask you to include a screenshot of the prompt that was used as well as the output that ChatGPT produced. The use of ChatGPT for any other homework problem is prohibited. This policy is enforced under the honor code.
<table>
<tr>
<th> <b>Homework</b></th>
<th> <b> Due date</b> </th>
<th> <b> Associated files</b> </th>
<th> <b> Solutions</b> </th><br/>
</tr>
{% for hwk in site.data.homework %}
<tr>
<td> <a href="assets/hwk/{{hwk.pset}}"> {{hwk.name}} </a></td>
<td> {{hwk.due_date}} </td>
</td>
{% if hwk.solns %}
<td>
  <a href="assets/hwk/{{hwk.solns}}"><b class="post-title">{{'Solutions'}}</b></a> 
</td>
{% else %}  
   <td> {{'-'}} </td>
  {% endif %}
  </tr>
  {%endfor%}
</table>


<td>{{day.topic}}
    {% if day.videos %}
    {% for v in day.videos %}
    <a href="http://rpdata.caltech.edu/courses/aph161/2021/videos/{{v.name}}">{{v.title}}</a><br/>
    {%endfor%}
    {%endif %}
    </td> 

