---
layout: landing
title: Events/Topics
description: イベント情報やトピック
image: assets/images/keeper1.jpeg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">
		<div class="row">

		{% for post in site.posts %}
		{% if post.title != 404 %}
		{% if post.tag != "training" %}

			<div class="6u 12u$(small)">
				<a href="{{ post.url }}">
					<header class="major">
						<h3>
						{{ post.title }}
						</h3>
					</header>
					<h2>
						{{ post.eventdate }}
					</h2>
					<p>
						{{ post.description }}
					</p>
				</a>
			</div>

		{% endif %}
		{% endif %}
		{% endfor %}

		</div>
	</div>
</section>

</div>
