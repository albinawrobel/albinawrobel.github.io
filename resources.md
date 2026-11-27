---
layout: default
title: Resources
description: Free, open-source articles on growth marketing and go-to-market strategy for tech startups, by Albina Wrobel.
permalink: /resources/
---


# Free <span class="hl">playbooks.</span>

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

## Tools

<ul class="list">
  <li>
    <span class="title-static">Free GTM tools</span> <span class="tag">coming soon</span>
    <p>Simple calculators and templates for checking your marketing numbers. In the works.</p>
  </li>
</ul>
