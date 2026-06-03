---
layout: page
permalink: /repositories/
title: repositories
description: Selected research and coursework repositories
nav: true
nav_order: 4
---

## GitHub Repositories

<div class="list-group">
  {% for repo in site.data.repositories.github_repos %}
    {% assign repo_parts = repo | split: '/' %}
    {% assign repo_name = repo_parts[1] %}
    {% assign repo_owner = repo_parts[0] %}
    <a href="https://github.com/{{ repo }}" target="_blank" rel="noopener noreferrer" class="list-group-item list-group-item-action d-flex justify-content-between align-items-center">
      <div>
        <h6 class="mb-1"><i class="fa-brands fa-github"></i> {{ repo_name }}</h6>
        <small class="text-muted">{{ repo_owner }}</small>
      </div>
      <span><i class="fa-solid fa-arrow-up-right-from-square fa-sm"></i></span>
    </a>
  {% endfor %}
</div>
