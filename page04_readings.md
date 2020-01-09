---
layout: page
title: Readings and Videos
img: readings.jpg # Add image post (optional)
permalink: readings 
sidebar: true
---

---

## Readings

As the course progresses, we will post papers we find interesting or that we
specifically mention in class. 

{% for pub in site.data.pubs %}
<li> <a style="text-decoration: none;" href="http://rpdata.caltech.edu/courses/aph161/protected/2020/papers/{{pub.fname}}"> <b>{{pub.title}}</b> by {{pub.authors}} in {{pub.journal}}, {{pub.year}}, {{pub.vol_iss}}.</a> {{pub.desc}}</li>
{% endfor %}



## Videos

<li> <a style="text-decoration: none;" href="https://www.youtube.com/watch?v=hRGg5it5FMI"> <b>Some Animals Are More Equal than Others: Keystone Species and Trophic Cascades</b> (an HHMI video) </a> </li>

