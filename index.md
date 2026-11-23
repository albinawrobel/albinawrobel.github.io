---
layout: default
title: Home
---

<p class="eyebrow">{{ site.tagline }}</p>

# Go-to-market without the guesswork.

<p class="lede">I'm {{ site.author.name }}. I write free, open-source playbooks on growth marketing for tech startups — the traps founders fall into, how to spot them early, and simple tools to check your numbers.</p>

<div class="actions">
  <a class="button" href="{{ '/resources/' | relative_url }}">Browse resources</a>
  <a class="button secondary" href="{{ '/contact/' | relative_url }}">Work with me</a>
</div>

## Latest articles

<ul class="list">
{% for post in site.posts limit:3 %}
  <li>
    <a class="title" href="{{ post.url | relative_url }}">{{ post.title }}</a> <time>{{ post.date | date: "%b %-d, %Y" }}</time>
    {% if post.description %}<p>{{ post.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

## Free tools

<ul class="list">
{% assign tools = site.pages | where: "tool", true %}
{% for t in tools %}
  <li>
    <a class="title" href="{{ t.url | relative_url }}">{{ t.title }}</a> <span class="tag">calculator</span>
    {% if t.description %}<p>{{ t.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
