---
layout: page
title: Border Literature Exhibit
permalink: /border-literature/
nav: true
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


[def]: ../objects/object_list.csv

## Items

{% for book in site.data.border-literature %}
	<div class="border-book">
		<h2>{{ book.title }}</h2>
		<p>{{ book.author }} — {{ book.edition }}</p>
		{% if book.image %}
			<img src="{{ book.image }}" alt="{{ book.title }}">
		{% endif %}
		<p>{{ book.description }}</p>
	</div>
{% endfor %}