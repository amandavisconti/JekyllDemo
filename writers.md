---
layout: page
title: Authors
---
All authors on this research project:

{% for person in site.people %}

* <a href="{{ site.baseurl }}{{ person.url }}">{{ person.name }}</a>

{% endfor %}
