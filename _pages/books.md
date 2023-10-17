---
layout: page
permalink: /books/
title: Books
description: I enjoy reading books and am documenting some recommendations here -- (Last Updated  October 15, 2023)
nav: true
nav_order: 4
---
<!-- # Reference code - https://github.com/cagrimmett/jekyll-tools/tree/master/reading-list -->
<div class="container">
  <!-- <div class="last-update">Last updated {{ site.data.books.lastupdate }}</div> -->
  {{ }}
  {% for entry in site.data.books.list %}
  <div class="year-container">
    <div class="year">
      <h4>{{ entry.year }}</h4>
      <div class="number">{{ entry.books | size }} books</div>
    </div>
    <div class="books">
      <ul class="reading-list {{ entry.year }}">
        {% for book in entry.books %}
        <li>
          <a href="{{ book.url }}" alt="_blank" rel="nofollow noopener">{{
            book.title
          }}</a>
          <span class="author">by {{ book.writer }}</span>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
  {% endfor %}
</div>