---
layout: archive
title: "Conferences"
permalink: /conferences/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

2018
==========

<table>
{% for post in site.conferences reversed %}
  <tr>{{ post.date | default: "1900-01-01" | date: "%Y" }}</tr>
  <tr>{% include publication.html %}</tr>
{% endfor %}
</table>
