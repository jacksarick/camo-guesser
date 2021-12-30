# patterns:
{% assign camo-patterns = site.static_files %}
{% for patten in camo-patterns %}
	* [{{ pattern.path }}]({{ site.baseurl }}{{ pattern.path }}) <img src="{{ site.baseurl }}{{ pattern.path }}" width="500" height="500">
{% endfor %}

v3.2