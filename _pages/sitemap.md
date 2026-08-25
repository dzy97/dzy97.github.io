---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all pages on this site. For robots, an [XML version]({{ base_path }}/sitemap.xml) is also available.

<h2>Pages</h2>
{% for post in site.pages %}
  {% if post.title and post.url != "/404.html" and post.url != "/sitemap/" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
