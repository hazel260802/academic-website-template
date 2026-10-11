---
title: "Learning Materials"
layout: page
permalink: /teaching/
---

# Learning Materials

{% if site.data.teaching.size > 0 %}
{% for group in site.data.teaching %}
<div class="section-card" markdown="0">
<h2>{{ group.section }}{% if group.term %} <span class="text-muted" style="font-size: 0.875rem; font-weight: 400;">({{ group.term }})</span>{% endif %}</h2>
<ul class="teaching-list">
{% for item in group.items %}
<li>
{% if item.course %}<strong>{{ item.course }}</strong>{% if item.title %}: {% endif %}{% endif %}{{ item.title }}{% if item.term %} ({{ item.term }}){% endif %}
{% if item.description %}<br><span class="text-muted">{{ item.description }}</span>{% endif %}
{% if item.links %}
<div class="pub-actions" style="margin-top: var(--space-2);">
{% for link in item.links %}<a href="{{ link.url }}" target="_blank" rel="noopener" class="btn-pill btn-link">{{ link.label }}</a>{% endfor %}
</div>
{% endif %}
</li>
{% endfor %}
</ul>
</div>
{% endfor %}
{% else %}
<p class="text-muted">No materials listed yet. Add entries to <code>_data/teaching.yml</code>.</p>
{% endif %}
