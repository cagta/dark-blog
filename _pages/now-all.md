---
title: all of my now updates
description: "all of my now updates"
og-type: website
permalink: /blog/now
---

{% for post in site.categories.now %}
{% include blog-listing.html %}
{% endfor %}