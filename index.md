---
layout: default
title: Home
---

<section class="hero">
<p class="eyebrow">{{ site.author.name }} · Growth marketer</p>
<h1>Every business needs its own model. <span class="hl">I help you find yours.</span></h1>
<p class="lede">I work with startups on their first go-to-market strategy, and help young builders get real feedback from the market so they can keep perfecting their craft.</p>
<div class="actions">
  <a class="button" href="{{ '/contact/' | relative_url }}">Let's talk</a>
  <a class="button secondary" href="{{ '/about/' | relative_url }}">My story</a>
</div>
</section>

<div class="facts">
  <div class="fact"><div class="k">Started at 15</div><div class="v">Ran marketing for a new dog daycare</div></div>
  <div class="fact"><div class="k">Year one</div><div class="v">Six figures in revenue</div></div>
  <div class="fact"><div class="k">How I work</div><div class="v">Learn by doing</div></div>
</div>

## What I help with

<div class="services">
  <div class="service"><h3>Market strategy</h3><p>Who you're really for, where they are, and why they'd choose you. The foundation everything else sits on.</p></div>
  <div class="service"><h3>Business model</h3><p>Shaping the model around how your customers actually buy, not how a template says they should.</p></div>
  <div class="service"><h3>Getting customers</h3><p>A focused plan to win your first customers, and a plan to keep them coming back.</p></div>
  <div class="service"><h3>Market feedback</h3><p>Getting your product in front of real people early, so you're building on what the market tells you.</p></div>
</div>

## My story, short version

<ol class="timeline">
  <li><span class="when">Age 15</span><p>My mom opened a dog daycare right before COVID hit. She wasn't very tech-savvy, so I took over everything digital, including marketing. I didn't know anything about marketing, so I learned by doing: I reframed our business model and built a customer acquisition and retention strategy that generated <strong>six figures in revenue in the first year</strong>. I stayed for over three years.</p></li>
  <li><span class="when">School</span><p>I shifted my focus to school and studied astrophysics at York University for two years.</p></li>
  <li><span class="when">Local businesses</span><p>I went back to growth marketing with small businesses in my neighbourhood, helping owners who weren't digital natives build their online presence and catch up with how the market had shifted. The biggest lesson: the hard part is earning trust and communicating clearly, not the tactics.</p></li>
  <li><span class="when">Now</span><p>I'm taking a year to work with startups, combining what I learned building a business from the ground up with my ability to communicate with people from all kinds of backgrounds.</p></li>
</ol>

<blockquote class="belief">The best way to learn is by doing.</blockquote>

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
