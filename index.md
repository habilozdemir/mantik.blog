---
layout: default
title: mantik.blog
---

# mantik.blog

## Habil Özdemir'in Kaleminden

<ul>
  {% for page in site.pages %}
    {% if page.name contains '.md' and page.name != 'index.md' and page.name != 'README.md' %}
      <li>
        <a href="{{ page.url | relative_url }}">
          {{ page.name | remove: '.md' | replace: '-', ' ' }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
