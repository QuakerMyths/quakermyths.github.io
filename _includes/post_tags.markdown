	Tags:
	<ul>
		{% for tag in page.tags %}
			<li><a href="/tags/{{ tag | replace:' ', '-' | downcase }}">{{ tag }}</a></li>
		{% endfor %}
	</ul>
