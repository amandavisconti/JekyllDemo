---
layout: default
---
<h2>{{ page.name }}</h2>

{{ content }}

<h2>Posts by {{ page.name }}:</h2>
{% for post in site.posts %}
{% if post.author == page.name %}
* <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>  
{% endif %}
{% endfor %}
