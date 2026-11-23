---
layout: default
title: Contact
description: Get in touch about go-to-market strategy and growth marketing for your startup.
permalink: /contact/
---

<p class="eyebrow">Contact</p>

# Let's talk.

<p class="lede">Working on go-to-market for a tech startup? Questions about something I wrote? Reach out.</p>

<div class="card">
  {% if site.booking_url != "" %}
  <p><strong>The fastest way:</strong> book a call directly.</p>
  <p><a class="button" href="{{ site.booking_url }}">Book a call</a></p>
  {% endif %}
  <ul class="contact-list">
    <li><span>Email</span> <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></li>
    {% if site.phone != "" %}<li><span>Phone</span> <a href="tel:{{ site.phone | remove: ' ' }}">{{ site.phone }}</a></li>{% endif %}
    {% if site.linkedin != "" %}<li><span>LinkedIn</span> <a href="{{ site.linkedin }}">{{ site.linkedin | remove: "https://" | remove: "www." }}</a></li>{% endif %}
    {% if site.github != "" %}<li><span>GitHub</span> <a href="https://github.com/{{ site.github }}">github.com/{{ site.github }}</a></li>{% endif %}
  </ul>
</div>
