---
layout: post
category: list
title: "Recent Reads "
date: 2017-01-22
thumb: main.png
hero: false
full: true
color: "#1ED760"
---
Here are some of books I've recenly enjoyed, in no particular order.

<ul class="list article-list list-grid list-grid-numbered list-shadow">
  {% for books in site.data.books limit:50 %}
  <li class="list-item">
    <a href="{{ books.link }}">
      <h5 class="list-rank"></h5>
      <img src="/img/{{ page.title | slugify }}/{{ books.title }}.jpg" class="list-image list-image-book">
      <h3>{{ books.title }}</h3>
      <h5>{{ books.author }}</h5>
    </a>
  </li>
  {% endfor %}
</ul>

