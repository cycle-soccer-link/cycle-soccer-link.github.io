---
layout: landing
title: Let's Get Started!
description: サイクルサッカーを始めよう！
image: assets/images/P1190720.jpeg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">


		{% for post in site.posts reversed %}
{% if post.title != 404 %}
{% if post.tag == "training" %}
	<a href="{{ post.url }}">
<header class="major">
<h3>
{{ post.title }}
</h3>
</header>
<p>
	{{ post.description }}
</p>
</a>
{% endif %}
{% endif %}
		{% endfor %}

	</div>
</section>

</div>
