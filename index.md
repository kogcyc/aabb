---
layout: index
title: Home
classes: zero
---

<ul>
  {% assign ordered_pages = site.pages | sort: 'order' %}
  {% for page in ordered_pages %}
  <div class="{{ page.collection }} {{ page.collection }}">
    <li>
      <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
      <p>{{ page.excerpt }}</p>
    </li>
  </div>
  {% endfor %}
</ul>
