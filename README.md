# patterns:

{% for file in site.static_files %}
  {% if file.path contains include.camo-patterns %}
    {% assign filenameparts = file.path | split: "/" %}
    {% assign filename = filenameparts | last | replace: file.extname,"" %}
    - {{ file }}
    - {{ filename }}
  {% endif %}
{% endfor %}