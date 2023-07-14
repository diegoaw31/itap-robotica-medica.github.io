---
title: "ITAP Medical Robotics - Team Photos"
layout: piclay
excerpt: "ITAP Medical Robotics -- Team Photos"
permalink: /teampictures/
---

# Team Pictures

{% assign number_printed = 0 %}
{% for teampic in site.data.teampictures %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div>
    <h4>{{ teampic.date }}</h4>
  </div>
  <div>
    <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ teampic.image }}" class="img-responsive" width="100%" style="float: bottom: 0" />
  </div>
  <div>
    <p>{{ teampic.caption}}</p>
  </div>
  <ul style="overflow: hidden">
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/escalada.JPG" width="60%">
</figure>


