---
title: "News"
layout: textlay
excerpt: "ITAP Medical Robotics -- News"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }}
<br>
<em>{{ article.headline }}</em>
<br><a href=article.link>{{ article.linkface }}</a></p>
{% endfor %}
