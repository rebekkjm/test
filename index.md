---
layout: default
title: Rebekka
---

Welcome to my blog.

<p>Bla bla</p>

[Email me](mailto:rebekka.morken@gmail.com "Email me")

[About](about/ "About")

[Pictures](pictures/ "Pictures")

{% for post in site.posts limit:5 %}
<!-- <h2><a href="{{ post.url }}">{{ post.title }}</a></h2> -->

<h2>{{ post.title }}</h2>

{{ post.content }}

<em>Posted on {{ post.date | date_to_long_string }}.</em>

{% endfor %}

