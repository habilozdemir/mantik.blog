<p style="text-align: center; color: #666; font-size: 1.1em; margin-bottom: 20px;">Habil Özdemir'in Kaleminden</p>
<style>footer.site-footer { display: none; }</style>
{% for page in site.pages %}{% if page.name contains '.md' and page.name != 'index.md' and page.name != 'README.md' and page.name != 'LICENSE.md' and page.name != 'LICENSE' %}
- [{{ page.name | remove: '.md' }}]({{ page.url | relative_url }})
{% endif %}{% endfor %}
