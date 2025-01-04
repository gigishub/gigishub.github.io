// filepath: /workspaces/gigishub.github.io/index.markdown
---
layout: default
title: Home
---

# Welcome to My Awesome Site

![Banner Image](path/to/your/banner-image.jpg)

## About This Site

This site is a showcase of my work and interests. Here you will find:

- **Blog Posts**: Insights and stories from my journey.
- **Projects**: A portfolio of my projects.
- **Contact**: Ways to get in touch with me.

## Latest Posts

{% for post in site.posts limit:3 %}
  - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}