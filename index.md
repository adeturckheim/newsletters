---
layout: default
title: Newsletters
---

# Newsletters

A small archive of newsletters.

## AI

{% assign ai_pages = site.pages | where_exp: "p", "p.path contains 'news/ai/'" | sort: "path" | reverse %}
{% for p in ai_pages %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

## Paris Restaurants

{% assign paris_pages = site.pages | where_exp: "p", "p.path contains 'news/paris_restaurants/'" | sort: "path" | reverse %}
{% for p in paris_pages %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}
