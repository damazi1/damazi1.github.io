---
layout: page
title: Projects
permalink: /projects/
---

## Moje projekty na GitHub
<ul>
  {% for repo in site.github.public_repositories %}
    {% unless repo.fork %}
      <li>
        <strong><a href="{{ repo.html_url }}">{{ repo.name }}</a></strong> — ⭐ {{ repo.stargazers_count }}<br>
        {{ repo.description }}
      </li>
    {% endunless %}
  {% endfor %}
</ul>