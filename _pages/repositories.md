---
layout: page
permalink: /repositories/
title: repositories
description: Selected research and coursework repositories
nav: true
nav_order: 4
---

## GitHub Repositories

<ul>
  {% for repo in site.data.repositories.github_repos %}
    <li>
      <a href="https://github.com/{{ repo }}" target="_blank" rel="noopener noreferrer"><strong>{{ repo }}</strong></a>
    </li>
  {% endfor %}
</ul>
