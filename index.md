---
layout: default
title: Home
---

<ul>
  {% assign ordered_pages = site.pages | sort: 'order' %}
  {% for page in ordered_pages %}
    <li>
      <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
      <p>{{ page.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
