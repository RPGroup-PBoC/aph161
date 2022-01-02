---
layout: page
title: Readings
img: readings.jpg # Add image post (optional)
permalink: readings 
sidebar: true
---

---

## Readings

As the course progresses, we will post papers we find interesting or that we
specifically mention in class. 

{% for pub in site.data.pubs %}
{% if  pub.fname %}
<li> <a style="text-decoration: none;" href="http://rpdata.caltech.edu/courses/aph161/protected/2022/papers/{{pub.fname}}"> <b>{{pub.title}}</b> by {{pub.authors}} in {{pub.journal}}, {{pub.year}}, {{pub.vol_iss}}.</a> {{pub.desc}}</li>
{% else %}
<li> <a style="text-decoration: none;" href="{{pub.url}}"> <b>{{pub.title}}</b>.</a> {{pub.desc}}</li>
{% endif %}
{% endfor %}

