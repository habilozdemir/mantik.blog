{% for post in site.pages %}
  - [{{ post.title | default: post.name }}]({{ post.url | relative_url }})
{% endfor %}
