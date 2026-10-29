---
layout: default
title: mantik.blog
---

# mantik.blog

## Habil Özdemir'in Kaleminden

<ul>
  {% assign sayfalar = site.pages | sort: 'name' %}
  {% for page in sayfalar %}
    {% if page.name contains '.md' and page.name != 'index.md' and page.name != 'README.md' %}
      <li>
        <a href="{{ page.url | relative_url }}">
          {{ page.name | remove: '.md' | replace: '-', ' ' }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

<br>
<hr>
<br>

Tüm yazılı içerikler [Creative Commons Atıf 4.0 Uluslararası Lisansı](https://creativecommons.org/licenses/by/4.0/deed.tr) ile lisanslanmıştır. Kaynak gösterilerek kullanılabilir.
