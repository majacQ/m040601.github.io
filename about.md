---
layout: page
title: About
permalink: /about/
---


epubs on mystaticfiles:
====

code
    {% for epubfile in site.static_files %}
    {% if epubfile.path contains 'mystaticfiles/epubs' %}
      <a href="{{site.baseurl}}{{epubfile.path}}">{{epubfile.path}} last modified on {{epubfile.modified_time}}</a>
    {% endif %}
    {% endfor %}

{% for epubfile in site.static_files %}
{% if epubfile.path contains 'mystaticfiles/epubs' %}
  <a href="{{site.baseurl}}{{epubfile.path}}">{{epubfile.path}} last modified on {{epubfile.modified_time}}</a>
{% endif %}
{% endfor %}

epubs on other places:
====

bla



### More Information

A place to include any other types of information that you'd like to include about yourself.

### Contact me

[email@domain.com](mailto:email@domain.com)
