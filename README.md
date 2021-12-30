# patterns:
{% assign camo-patterns = site.static_files | where: "image", true %}

<ul>
{% for pattern in site.camo-patterns %}
	<li> {{ pattern }}</li>
{% endfor %}
</ul>

v3