---
layout: default
title: Resources
description: Free, open-source articles and calculators on growth marketing and go-to-market strategy for tech startups.
permalink: /resources/
---

<p class="eyebrow">Resources</p>

# Free playbooks & tools

<p class="lede">Everything here is free and open source. Use it, share it, adapt it for your own team.</p>

## Articles

<ul class="list">
{% for post in site.posts %}
  <li>
    <a class="title" href="{{ post.url | relative_url }}">{{ post.title }}</a> <time>{{ post.date | date: "%b %-d, %Y" }}</time>
    {% if post.description %}<p>{{ post.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

## Tools & calculators

<ul class="list">
{% assign tools = site.pages | where: "tool", true %}
{% for t in tools %}
  <li>
    <a class="title" href="{{ t.url | relative_url }}">{{ t.title }}</a> <span class="tag">calculator</span>
    {% if t.description %}<p>{{ t.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
