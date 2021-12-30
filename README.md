# patterns:
{% assign camo-patterns = site.static_files | where: "image", true %}

<ul>
{% for pattern in site.camo-patterns %}
	<li> {{ pattern.path }} <img src="{{ pattern.path }}" width="500" height="500"> </li>
{% endfor %}
</ul>

v3.1