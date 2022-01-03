---
title: "ITAP Medical Robotics - Projects"
layout: gridlay
excerpt: "ITAP Medical Robotics -- Projects"
sitemap: false
permalink: /projects/
---


# Projects

{% assign number_printed = 0 %}
{% for proj in site.data.projectlist %}

<div style="padding-left:15px;padding-right:15px;">
<div class="well" style="overflow: hidden;">
<img src="{{ site.url }}{{ site.baseurl }}/images/projpic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
<pubtit><a href="{{ site.url }}{{ site.baseurl }}/projects/{{ proj.url }}">{{ proj.title }}</a></pubtit>
<p>{{ proj.description }}</p>
</div>
</div>


{% endfor %}

<p> &nbsp; </p>