---
layout: page
permalink: /books/
title: Books
description: Books that I have read recently!
nav: true
nav_order: 3
---

{% for book in site.data.books %}
  <li>
      {{ book.title }}
      <ul>
        <li style="list-style: none;"> Writer - {{ book.writer }}</li>
        <li style="list-style: none;"> <a href="{{ book.url }}">LINK</a></li>
      </ul>     
  </li>
{% endfor %}

