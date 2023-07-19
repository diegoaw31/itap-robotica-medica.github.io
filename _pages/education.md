---
title: "ITAP Medical Robotics - Education"
layout: gridlay
excerpt: "ITAP Medical Robotics -- Education."
sitemap: false
permalink: /education/
---


# Education

<!-- ## Current student projects -->

{% for file in site.data.education %}

  {% if file.state == 0 %} 
  
  {{ file.title }}<br />
  <b>Autor: </b>{{ file.author }}<b> Tutor: </b>{{ file.tutor }}<b> Año: </b>{{ file.year }}<br />
  <b>Titulación: </b>{{ file.studies }} <br  />
    
  {% endif %}
  
{% endfor %}


## Completed student projects

{% for file in site.data.education %}

  {% if file.state == 1 %} 
  
  {{ file.title }} (Oculto)<br>
  <b>Autor: </b>{{ file.author }}<b> Tutor: </b>{{ file.tutor }}<b> Año: </b>{{ file.year }}<br />
  <b>Titulación: </b>{{ file.studies }} <br  />
  
  {% endif %}

  {% if file.state == 2 %}
  
  <a target="_blank" href="{{ file.url }}">{{ file.title }}</a><br>
  <b>Autor: </b>{{ file.author }}<b> Tutor: </b>{{ file.tutor }}<b> Año: </b>{{ file.year }}<br />
  <b>Titulación: </b>{{ file.studies }} <br  />
  
  {% endif %}
  
{% endfor %}


<!--

<p> &nbsp; </p>


Jump to: [Leiden](#leiden), [ETHZ](#ethz), [Cornell](#cornell), [St Andrews](#st-andrews)

## Leiden

#### Timelapse of our STM assembling [(see LION news item)](https://www.physics.leidenuniv.nl/index.php?id=11573&news=867&type=lion&ln=EN):
<iframe width="560" height="315" src="https://www.youtube.com/embed/3iKvUMv1h5A" frameborder="0" allowfullscreen></iframe>

#### Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

First advertisement.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageLeiden_red.jpg" width="60%" >
</figure>


## ETHZ
From the [group of Andreas Wallraff](http://www.qudev.ethz.ch/).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageETH_red.jpg" width="60%">
</figure>

## Cornell
From the [group of Seamus JC Davis](http://davisgroup.lassp.cornell.edu).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageCornell_red.jpg" width="60%">
</figure>

## St Andrews
From the [group of Felix Baumberger](http://dqmp.unige.ch/baumberger/) (now at University of Geneva).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageSTA_red.jpg" width="60%">
</figure>

-->
