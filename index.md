---
layout: index_layout
title: Home
classes: _kontent
---

<div class="logoDIV">
  <a
    href="."
    title="click here to go to the home page"
    class="logo"
  >
    kogswell
  </a>
</div>

<ul>
  {% assign ordered_pages = site.pages | sort: 'order' %}
  {% for page in ordered_pages %}
  <div class="{{ page.collection }} {{ page.classes }}">
    <li>
       <div class="title"><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></div>
      <p>{{ page.excerpt }}</p>
    </li>
  </div>
  {% endfor %}
</ul>





