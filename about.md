---
layout: page
title: About
permalink: /about/
---


epubs:
====

start epubs:

{% for epub in site.static_files %}
{% if epub.path contains 'epub' %}
  <a href="{{site.baseurl}}{{epub.path}}">{{epub.path}} last modified on {{epub.modified_time}}</a>
{% endif %}
{% endfor %}

Some information about you!


Stop epubs
### More Information

A place to include any other types of information that you'd like to include about yourself.

### Contact me

[email@domain.com](mailto:email@domain.com)
