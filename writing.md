---
layout: single
title: "Writing"
permalink: /writing/
author_profile: true
---

Articles on engineering leadership, capital investment, energy transition, and the structural patterns that determine whether major industrial projects succeed.

I publish roughly quarterly — quality over quantity.

## Articles

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})** — {{ post.date | date: "%B %Y" }}
  <br><em>{{ post.excerpt | strip_html | truncatewords: 25 }}</em>
{% endfor %}

{% if site.posts.size == 0 %}
*First articles publishing soon.*
{% endif %}
