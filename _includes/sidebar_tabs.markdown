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
			{% for category in site.my_categories %}
				<li><a href="/category/{{ category.slug }}">{{ category.name }}</a></li>
			{% endfor %}
		</ul>
	</section>
	<section>
		<h4>Tags</h4>
		<ul>
			{% for tag in site.my_tags %}
				<li><a href="/tag/{{ tag.slug }}">{{ tag.name }}</a></li>
			{% endfor %}
		</ul>
	</section>
