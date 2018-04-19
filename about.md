---
layout: page
title: About
permalink: /about/
---



epubs on mystaticfiles:
====
{% for epubfile in site.static_files %}
{% if epubfile.path contains 'mystaticfiles/epubs' %}
  <a href="{{site.baseurl}}{{epubfile.path}}">{{epubfile.path}}</a> , last modified on {{epubfile.modified_time}}
{% endif %}
{% endfor %}


txts on mystaticfiles:
====
{% for txtfile in site.static_files %}
{% if txtfile.path contains 'txt' %}
  <a href="{{site.baseurl}}{{epub.path}}">{{txtfile.path}}</a> , last modified on {{txtfile.modified_time}}
{% endif %}
{% endfor %}
