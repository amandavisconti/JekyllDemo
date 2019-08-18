---
layout: default
---
{{ page.name }}

{{ content }}

Posts by {{ page.name }}:
{% for post in site.posts %}
{% if post.author == page.name %}
* <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>  
{% endif %}
{% endfor %}
