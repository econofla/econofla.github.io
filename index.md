---
layout: home
title: "Silicon Economics Review"
---

Welcome to **Silicon Economics Review**: independent, data-driven analysis on the global silicon industry: wafers, semiconductor fabrication, packaging, capital expenditure cycles, and supply chains.

Below you'll find our latest reviews. For our approach, see [Methodology](/methodology).
<div class="hero">
	<h1>Silicon Economics Review</h1>
	<p class="subtitle">Independent, data-driven analysis of the global silicon industry</p>
	<ul class="hero-tags">
		<li>Wafers</li>
		<li>Semiconductor Fabs</li>
		<li>Packaging</li>
		<li>Capex Cycles</li>
		<li>Supply Chains</li>
	</ul>
</div>

<!-- <section class="featured-intro">
	<p>
		Welcome to <strong>Silicon Economics Review</strong>, your source for in-depth reviews and insights on the silicon industry. We cover everything from wafer markets to advanced packaging, global fab construction, and the economics driving semiconductor supply chains.
	</p>
	<p>
		<a class="btn" href="/methodology">See our methodology</a>
	</p>
</section> -->

<section class="latest-reviews">
	<h2>Latest Reviews</h2>
	<ul class="post-list">
		{% for post in site.posts limit:6 %}
			<li class="post-card">
				<a href="{{ post.url | relative_url }}">
					<h3>{{ post.title }}</h3>
					<span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
					<p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
				</a>
			</li>
		{% endfor %}
	</ul>
</section>
