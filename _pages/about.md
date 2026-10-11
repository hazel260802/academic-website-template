---
title: "About"
layout: page
permalink: /about/
---

# About

<div class="section-card">
<div class="pi-card">
<img src="{{ site.photo | prepend: '/images/' | relative_url }}" class="pi-photo" alt="{{ site.name }}" width="160" height="160">
<div>
<h2 class="pi-name">{{ site.name }}</h2>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email" aria-label="Email">{% include icon.html name="envelope" %}</a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.links.cv | prepend: '/' | relative_url }}" class="icon-link" title="CV" aria-label="CV">{% include icon.html name="cv" %}</a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar" aria-label="Google Scholar">{% include icon.html name="google-scholar" %}</a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub" aria-label="GitHub">{% include icon.html name="github" %}</a>{% endif %}
{% if site.links.researchgate and site.links.researchgate != "" %}<a href="{{ site.links.researchgate }}" class="icon-link" title="ResearchGate" aria-label="ResearchGate">{% include icon.html name="researchgate" %}</a>{% endif %}
</div>
{% if site.data.pi[0].education %}
<ul style="margin-top: var(--space-4);">
{% for education in site.data.pi[0].education %}
<li>{{ education | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
{% endif %}
</div>
</div>
</div>

{% assign phd = site.data.pi[0].phd %}
{% if phd %}
<div class="section-card" markdown="0">
<h3>PhD Thesis</h3>
<p><strong>{{ phd.title }}</strong>{% if phd.title_fr %}<br><em>{{ phd.title_fr }}</em>{% endif %}</p>
{% if phd.summary %}<p>{{ phd.summary }}</p>{% endif %}
<ul>
{% if phd.degree %}<li><strong>Degree:</strong> {{ phd.degree }}</li>{% endif %}
{% if phd.institutions %}<li><strong>Institutions:</strong> {{ phd.institutions }}</li>{% endif %}
{% if phd.labs %}<li><strong>Laboratories:</strong> {{ phd.labs }}</li>{% endif %}
{% if phd.doctoral_school %}<li><strong>Doctoral school:</strong> {{ phd.doctoral_school }}</li>{% endif %}
{% if phd.supervisors and phd.supervisors.size > 0 %}<li><strong>Supervisors:</strong> {{ phd.supervisors | join: ", " }}</li>{% endif %}
{% if phd.start %}<li><strong>Started:</strong> {{ phd.start }}</li>{% endif %}
</ul>
{% if phd.notes or phd.code %}
<div class="pub-actions">
{% if phd.notes %}<a href="{{ phd.notes }}" target="_blank" rel="noopener" class="btn-pill btn-link">Learning notes</a>{% endif %}
{% if phd.code %}<a href="{{ phd.code }}" target="_blank" rel="noopener" class="btn-pill btn-git">GitHub</a>{% endif %}
</div>
{% endif %}
</div>
{% endif %}

{% if site.data.grants %}
<div class="section-card">
<h3>Grants</h3>
<ul>
{% for grant in site.data.grants %}
<li>{{ grant.name }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.awards %}
<div class="section-card">
<h3>Awards</h3>
<ul>
{% for award in site.data.awards %}
<li>{% if award.url %}<a href="{{ award.url }}" target="_blank" rel="noopener">{{ award.name }}</a>{% else %}{{ award.name }}{% endif %}{% if award.detail %} {{ award.detail }}{% endif %}</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.funders %}
<div class="section-card">
<h4>Sponsors</h4>
<div class="sponsor-logos" style="display: flex; flex-wrap: wrap; align-items: center; justify-content: center; gap: var(--space-6);">
{% for funder in site.data.funders %}
<a href="{{ funder.url }}" target="_blank"><img src="{{ funder.image | prepend: '/images/' | relative_url }}" alt="Funder logo" style="max-height: 80px; max-width: 200px; border-radius: 0;" loading="lazy"></a>
{% endfor %}
</div>
</div>
{% endif %}
