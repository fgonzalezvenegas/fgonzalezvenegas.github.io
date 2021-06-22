---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

# Journal articles

{% for post in site.publications reversed %}
{if post.collection == 'publications'}
  {% include archive-single.html %}
{% endfor %}

# Working papers

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}

# International conferences

{% for post in site.confs reversed %}
  {% include archive-single.html %}
{% endfor %}