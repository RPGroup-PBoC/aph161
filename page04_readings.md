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
{% for day in site.data.pubs %}
## {{day[0]}}
{% for pub in day[1] %}
{% if  pub.fname %}
<li> <a style="text-decoration: none;" href="http://rpdata.caltech.edu/courses/aph161/protected/2022/papers/{{pub.fname}}" target="_blank"> <b>{{pub.title}}</b> by {{pub.authors}} in {{pub.journal}}, {{pub.year}}, {{pub.vol_iss}}.</a> {{pub.desc}}</li>
{% else %}
<li> <a style="text-decoration: none;" href="{{pub.url}}" target="_blank"> <b>{{pub.title}}</b>.</a> {{pub.desc}}</li>
{% endif %}
{% endfor %}
{% endfor %}

