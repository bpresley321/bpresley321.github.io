---
layout: default
title: Writing
---

{% include nav.html %}

Welcome. This is a small personal site for notes, little tools, and links I use myself. My [start page](https://start-page-v1-remd.vercel.app) is the best place to begin.

## Writing

{% for post in site.posts %}
- {{ post.date | date: "%b %-d, %Y" }} &mdash; [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
