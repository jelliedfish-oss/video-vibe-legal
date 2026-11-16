---
layout: default
title: Video Vibe
home: true
---
<p class="eyebrow">App information</p>
<h1>Video Vibe</h1>
<p class="intro">Privacy information and legal documents for the Video Vibe app, in one place.</p>

{% assign privacy_page = site.pages | where: 'name', 'privacy.md' | first %}
<a class="policy-card" href="{{ '/privacy/' | relative_url }}">
  <span>
    <span class="card-title">Privacy Policy</span>
    <span class="card-detail">{% if privacy_page.policy_status == 'pending' %}Policy content will be published here.{% else %}Read how Video Vibe handles your information.{% endif %}</span>
  </span>
  <span class="card-arrow" aria-hidden="true">↗</span>
</a>
