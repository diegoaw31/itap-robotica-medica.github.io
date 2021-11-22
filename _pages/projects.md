---
title: "ITAP Medical Robotics - Projects"
layout: gridlay
excerpt: "ITAP Medical Robotics -- Projects."
sitemap: false
permalink: /projects/
---


# Projects

{% assign number_printed = 0 %}
{% for publi in site.data.projectlist %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}


<div style="padding-left:15px;padding-right:15px;"> <!--<div class="col-sm-6 clearfix">-->
<div class="well">
### <pubtit><a href="{{ site.url }}{{ site.baseurl }}/projects/{{ publi.url }}">{{ publi.title }}</a></pubtit>
<p>{{ publi.description }}</p>
</div>
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

<p> &nbsp; </p>