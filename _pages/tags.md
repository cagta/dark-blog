---
title: "tags"
description: "all of my blog posts sorted by tag"
permalink: /blog/tags
---

{% include search.html %}

<h2 id="categories">categories</h2>
<div class="tag-list">
<a href="/blog">essays ({{ site.categories.essays | size }})</a>
<a href="/blog/now">now ({{ site.categories.now | size }})</a>
<a href="/notes">recent notes</a>
</div>

<h2 id="tags">tags</h2>

{% assign sortedTags = site.tags | sort %}

<div class="tag-list">
{% for tag in sortedTags %}
	<a href="#{{tag[0]}}">{{ tag[0] }}&nbsp;({{ tag[1] | size }})</a>
{% endfor %}
</div>

{% for tag in sortedTags %}

<h2 id="{{ tag[0] }}">{{ tag[0] }}</h2>

{% for post in tag[1] %}
	{% include blog-listing.html %}
{% endfor %}

<p><a href="#" class="internal-link">all tags &#8593;</a></p>

{% endfor %}
