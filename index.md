---
layout: default
title: Home
---

<section class="hero">
<p class="eyebrow">{{ site.author.name }} · Growth marketer</p>
<h1>I help tech startups <span class="hl">go to market.</span></h1>
<p class="lede">Hi, I'm Albina. I've been doing growth marketing since I was 15, and now I work with new startups on finding their first customers and getting the go-to-market right.</p>
<div class="actions">
  <a class="button" href="{{ '/contact/' | relative_url }}">Let's talk</a>
  <a class="button secondary" href="{{ '/about/' | relative_url }}">More about me</a>
</div>
</section>

<div class="facts">
  <div class="fact"><div class="k">Started</div><div class="v">Growth marketing at 15</div></div>
  <div class="fact"><div class="k">Studied</div><div class="v">Astrophysics, York University</div></div>
  <div class="fact"><div class="k">Now</div><div class="v">Helping startups go to market</div></div>
</div>

## What I'm about

I got into growth marketing during the pandemic, when everything went digital overnight, and learned it by doing it. After two years studying astrophysics, I'm back in it full time, working with early-stage startups and writing openly about the traps I see founders fall into.

## Latest articles

<ul class="list">
{% for post in site.posts limit:3 %}
  <li>
    <a class="title" href="{{ post.url | relative_url }}">{{ post.title }}</a> <time>{{ post.date | date: "%b %-d, %Y" }}</time>
    {% if post.description %}<p>{{ post.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

<div class="actions">
  <a class="button secondary" href="{{ '/resources/' | relative_url }}">All resources →</a>
</div>
