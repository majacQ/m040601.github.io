---
layout: page
title: About
permalink: /about/
---



epubs on mystaticfiles:
====
{% for epubfile in site.static_files %}
{% if epubfile.path contains 'mystaticfiles/epubs' %}
  <a href="{{site.baseurl}}{{epubfile.path}}">{{epubfile.path}} last modified on {{epubfile.modified_time}}</a>
{% endif %}
{% endfor %}



epubs on other places:
====
{% for epub in site.static_files %}
{% if epub.path contains 'epub' %}
  <a href="{{site.baseurl}}{{epub.path}}">{{epub.path}} last modified on {{epub.modified_time}}</a>
{% endif %}
{% endfor %}


codey:
====

```
{% for epubfile in site.static_files %}
{% if epubfile.path contains 'mystaticfiles/epubs' %}
  <a href="{{site.baseurl}}{{epubfile.path}}">{{epubfile.path}} last modified on {{epubfile.modified_time}}</a>
{% endif %}
{% endfor %}
```

```
{% for epub in site.static_files %}
{% if epub.path contains 'epub' %}
  <a href="{{site.baseurl}}{{epub.path}}">{{epub.path}} last modified on {{epub.modified_time}}</a>
{% endif %}
{% endfor %}
```

