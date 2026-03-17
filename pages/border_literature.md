---
layout: page
title: Border Literature Exhibit
permalink: /border-literature/
nav: true
gallery: true
---

## Overview

This exhibit presents novels, literary works, and their metadata in relation to border literature themes. Please click on the novel to see the full cover. 


## Curatorial Notes

[Add reflections or interpretive text about the exhibit.]

## Border Literature Exhibit

<div class="border-gallery">
{% for row in site.data.border_literature %}
  <div class="border-book-item">
    <a class="spotlight gallery-img" href="{{ row.image }}" title="{{ row.title | replace: '"', '&quot;' }}">
      <img src="/assets/images/covers/thumbs/{{ row.objectid }}_th.jpg" alt="{{ row.title | replace: '"', '&quot;' }}">
    </a>
    <div class="book-info">
      <h3>{{ row.title }}</h3>
      <p class="byline">{{ row.author }} — {{ row.edition }}</p>
      <p class="genre">{{ row.genre }}</p>
    </div>
  </div>
{% endfor %}
</div>