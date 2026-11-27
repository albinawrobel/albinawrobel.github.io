---
layout: default
title: Resources
description: Free, open-source articles on growth marketing and go-to-market strategy for tech startups, by Albina Wrobel.
permalink: /resources/
---

# Articles, tools, <span class="hl">and guides.</span>

<p class="lede">Everything here is open source. Share it, quote it, make content from it, adapt it for your own work. I don't care as long as you make use of it.</p>

{% include resource-sections.html %}

<div class="section-head">
  <h2>Guides</h2>
  {% if guides.size > 3 %}<a class="see-all" href="{{ '/resources/guides/' | relative_url }}">Explore all guides →</a>{% endif %}
</div>

{% include resource-items.html items=guides limit="3" empty_title="Quick GTM guides" empty_text="Short, step-by-step guides you can use in under five minutes. In the works." %}

<div class="section-head">
  <h2>Articles</h2>
  {% if articles.size > 3 %}<a class="see-all" href="{{ '/resources/articles/' | relative_url }}">Explore all articles →</a>{% endif %}
</div>

{% include resource-items.html items=articles limit="3" empty_title="Articles" empty_text="Longer reads on go-to-market strategy. In the works." %}

<div class="section-head">
  <h2>Tools</h2>
  {% if tools.size > 3 %}<a class="see-all" href="{{ '/resources/tools/' | relative_url }}">Explore all tools →</a>{% endif %}
</div>

{% include resource-items.html items=tools limit="3" empty_title="Free GTM tools" empty_text="Simple calculators and templates for checking your marketing numbers. In the works." %}
