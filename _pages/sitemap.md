---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

<h2>Pages</h2>
<ul>
  <li><a href="{{ base_path }}/">About</a></li>
  <li><a href="{{ base_path }}/publications/">Publications</a></li>
</ul>

<h2>Publication Records</h2>
{% assign publications = site.publications | sort: "order" %}
<ul>
  {% for publication in publications %}
    <li>{{ publication.title }} ({{ publication.year }})</li>
  {% endfor %}
</ul>
