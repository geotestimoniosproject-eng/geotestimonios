---
layout: page
title: Border Literature Exhibit
permalink: /border-literature/
nav: true
gallery: true
---

## Overview

This exhibit presents novels, literary works, and their metadata in relation to border literature themes.

## Covers and Metadata

Each item includes:
- Author
- Edition
- Title
- Keywords


## Curatorial Notes

[Add reflections or interpretive text about the exhibit.]

## Gallery

<div class="border-gallery">
{% for row in site.data['border-literature - Sheet1'] %}
  <div class="border-book-item">
    <a class="spotlight gallery-img" href="{{ row.image }}" title="{{ row.title }}">
      <img src="/assets/images/covers/thumbs/{{ row.objectid }}_th.jpg" alt="{{ row.title }}">
    </a>
    <div class="book-info">
      <h3>{{ row.title }}</h3>
      <p class="byline">{{ row.author }} — {{ row.edition }}</p>
    </div>
  </div>
{% endfor %}
</div>