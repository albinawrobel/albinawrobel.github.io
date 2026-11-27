---
layout: default
---

<section class="hero">
<h1>Every business needs its own model. I help you find yours.</h1>
<p class="lede">I work with startups on their first go-to-market strategy, and help young builders get real feedback from the market so they can keep perfecting their craft.</p>
</section>

<div class="gtm" role="img" aria-label="The go-to-market loop: build the product, go to market, get feedback, and repeat.">
  <p class="gtm-label">The go-to-market loop</p>
  <div class="gtm-steps">
    <div class="gtm-step s1"><span class="n">01</span><h3>Build the product</h3><p>Make something for a real problem.</p></div>
    <div class="gtm-arrow" aria-hidden="true">→</div>
    <div class="gtm-step s2"><span class="n">02</span><h3>Go to market</h3><p>Put it in front of the right people.</p></div>
    <div class="gtm-arrow" aria-hidden="true">→</div>
    <div class="gtm-step s3"><span class="n">03</span><h3>Get feedback</h3><p>Learn what the market actually thinks.</p></div>
  </div>
  <div class="gtm-return" aria-hidden="true"><span>↺ Repeat. The feedback shapes what you build next.</span></div>
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
  <li><span class="when">Local businesses</span><p>I went back to growth marketing with small businesses in my neighbourhood. Most of the owners were Gen X or boomers who, like my mom, weren't very tech-savvy. Communication was the hardest part: they didn't trust the digital market and didn't know enough about it to see what it could do for them, so even a great strategy went nowhere if I couldn't explain it in their terms. That's where I learned communication isn't extra. It's the foundation every strategy is built on.</p></li>
  <li><span class="when">Now</span><p>I'm taking a year to work with startups, combining what I learned building a business from the ground up with my ability to communicate with people from all kinds of backgrounds.</p></li>
</ol>

<blockquote class="belief">The best way to learn is by doing.</blockquote>

## Latest articles

{% assign latest_articles = site.posts | where_exp: "p", "p.type != 'guide'" %}
<ul class="list">
{% for post in latest_articles limit:3 %}
  <li>
    <a class="title" href="{{ post.url | relative_url }}">{{ post.title }}</a> <time>{{ post.date | date: "%b %-d, %Y" }}</time>
    {% if post.description %}<p>{{ post.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

<div class="actions">
  <a class="button secondary" href="{{ '/resources/' | relative_url }}">All resources →</a>
</div>
