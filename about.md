---
layout: page
title: About
permalink: /about/
---

Jan24 2024-01-22


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
{% if txtfile.path contains 'mystaticfiles/txts' %}
  <a href="{{site.baseurl}}{{txtfile.path}}">{{txtfile.path}}</a> , last modified on {{txtfile.modified_time}}
{% endif %}
{% endfor %}


pdfs on mystaticfiles:
====
{% for pdffile in site.static_files %}
{% if pdffile.path contains 'mystaticfiles/pdfs' %}
  <a href="{{site.baseurl}}{{pdffile.path}}">{{pdffile.path}}</a> , last modified on {{pdffile.modified_time}}
{% endif %}
{% endfor %}



zims on mystaticfiles:
====
{% for zimfile in site.static_files %}
{% if zimfile.path contains 'mystaticfiles/zims' %}
  <a href="{{site.baseurl}}{{zimfile.path}}">{{zimfile.path}}</a> , last modified on {{zimfile.modified_time}}
{% endif %}
{% endfor %}


