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
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ teampic.image }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
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

--------
{% assign number_printed = 0 %}
{% for picture in site.data.teampictures %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ picture.link }}" class="img-responsive" width="70%" style="float: bottom" />
  <h4>{{ picture.caption }}</h4>
  <ul style="overflow: hidden">

{% if even_odd == 1 %}
</div>
{% endif %}

{% assign even_odd = number_printed | plus: 1 %}
    
{% endfor %}

{% if even_odd == 0 %}
</div>
{% endif %}


Escalada 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/escalada.JPG" width="60%">
</figure>


