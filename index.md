---
layout: default
title: Home
---

<section class="hero">
<p class="eyebrow">{{ site.tagline }}</p>
<h1>Go-to-market <span class="hl">without the guesswork.</span></h1>
<p class="lede">I'm {{ site.author.name }}. I write free, open-source playbooks on growth marketing for tech startups: the <span class="mark">traps founders fall into</span>, how to spot them early, and simple tools to check your numbers.</p>
<div class="actions">
  <a class="button" href="{{ '/resources/' | relative_url }}">Browse resources</a>
  <a class="button secondary" href="{{ '/about/' | relative_url }}">About me</a>
</div>
</section>

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
