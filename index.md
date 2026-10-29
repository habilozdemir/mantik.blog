{% assign sorted_pages = site.pages | sort: "name" %}
{% for page in sorted_pages %}{% if page.name contains '.md' and page.name != 'index.md' and page.name != 'README.md' and page.name != 'LICENSE.md' and page.name != 'LICENSE' %}
- [{{ page.name | remove: '.md' }}]({{ page.url | relative_url }})
{% endif %}{% endfor %}
