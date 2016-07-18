---
layout: post
title: You're up and running!
---

Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.

Assuming you have your gallery images in a structure like
====

    -img
      -gallery
        -image1.png
        -image2.png
        
    etc.
you can access them in a collection or page like this:

Start images:
====
{% for image in site.static_files %}
{% if image.path contains 'img/gallery' %}
  <p>{{image.path}} - {{image.modified_time}}</p>
  <img src="{{site.baseurl}}{{image.path}}">
{% endif %}
{% endfor %}
Stop images:

Start epubs:
====
{% for epub in site.static_files %}
{% if epub.path contains 'epub/gallery' %}
  <p>{{epub.path}} - {{epub.modified_time}}</p>
  <a href="{{site.baseurl}}{{epub.path}}">
{% endif %}
{% endfor %}
Stop epubs

This goes through all static files and check for a certain path (img/gallery in this example).
====

Than you can access the static file metadata for that file. (I named it 'image' in this example but you can name it whatever you want after the for keyword).

I think it doesn't make too much sense to put something like this in a blog post but rather in a page or a collection.
