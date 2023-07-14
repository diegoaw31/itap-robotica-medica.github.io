---
title: "ITAP Medical Robotics - Team Photos"
layout: piclay
excerpt: "ITAP Medical Robotics -- Team Photos"
permalink: /teampictures/
---

# Team Pictures

{% assign number_printed = 0 %}
{% for picture in site.data.teampictures %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ picture.caption }}</h4>
  <ul style="overflow: hidden">
{% endfor %}

Escalada 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/escalada.JPG" width="60%">
</figure>


