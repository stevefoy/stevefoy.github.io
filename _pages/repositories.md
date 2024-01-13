---
layout: page
permalink: /repositories/
title: repositories
description: Needs Updating of the `_data/repositories.yml` and `github_users` and `github_repos` of my repos.
nav: true
nav_order: 4
---

## GitHub Repositories

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
