<style>ul { list-style-type: none; padding-left: 0; }</style>
{% for file in site.static_files %}{% if file.extname == ".md" and file.name != "index.md" and file.name != "README.md" %}
- [{{ file.basename }}]({{ file.path | relative_url }})
{% endif %}{% endfor %}
