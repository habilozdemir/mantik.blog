{% for file in site.static_files %}{% if file.extname == ".md" and file.name != "index.md" and file.name != "README.md" and file.name != "LICENSE.md" and file.name != "LICENSE" %}
- [{{ file.basename }}]({{ file.path | relative_url }})
{% endif %}{% endfor %}
