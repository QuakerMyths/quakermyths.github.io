	<section>
		<h4>Recent</h4>
		<ul>
			{% for post in site.posts limit: 5 %}
				<li><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
			{% endfor %}
		</ul>
	</section>
	<section>
		<h4>Categories</h4>
		<ul>
			{% for topic in site.iterable.categories %}
				<li><a href="/categories/{{ topic.name }}">{{ topic.name }}</a></li>
			{% endfor %}
		</ul>
	</section>
	<section>
		<h4>Tags</h4>
		<ul>
			{% for topic in site.iterable.tags %}
				<li><a href="/tags/{{ topic.name | replace:' ','-' | downcase }}">{{ topic.name }}</a></li>
			{% endfor %}
		</ul>
	</section>
