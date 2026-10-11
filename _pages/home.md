---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Blockchain</a>
<a href="{{ '/research' | relative_url }}" class="chip">Zero-Knowledge Proofs</a>
<a href="{{ '/research' | relative_url }}" class="chip">Privacy-Preserving Systems</a>
<a href="{{ '/research' | relative_url }}" class="chip">Cybersecurity</a>
<a href="{{ '/research' | relative_url }}" class="chip">Bioinformatics</a>
<a href="{{ '/research' | relative_url }}" class="chip">IoT &amp; SDN</a>
<a href="{{ '/research' | relative_url }}" class="chip">AI for Networks</a>
</div>

I am a computer engineer and Master 2 student in computer and network systems at Université d'Évry Paris-Saclay.
My research covers secure healthcare data sharing, blockchain-based genomic data management, and privacy-preserving systems built on cryptography, including zero-knowledge proofs.
I work at the [IBISC Laboratory](https://www.ibisc.univ-evry.fr/) under Prof. Nazim Agoulmine on decentralized solutions for medical IoT devices and trustworthy data-sharing ecosystems.

<div class="callout callout-success" markdown="0">
<div class="callout-title">{% include icon.html name="award" class="callout-icon" %} Looking for a PhD position</div>
<p>I am looking for a PhD topic in cybersecurity, distributed network systems, or artificial intelligence applied to network systems. Feel free to <a href="mailto:{{ site.email }}">get in touch</a>.</p>
</div>

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

## About me

I received my engineering degree in computer science (5-year programme completed in 4 years) from the PFIEV elite programme at Hanoi University of Science and Technology (HUST) in 2024, graduating 5th of 40.
At HUST's BKCS lab I worked with Prof. Tran Hai-Anh on multi-objective deep reinforcement learning for edge-cloud server selection, published at IEEE Cloud Summit 2024.
In 2025 I joined Universidade do Porto (FEUP) as an Erasmus+ researcher, working with Prof. Mariana Cunha and Prof. João P. Vilela on context-aware location privacy for multimodal transportation.

Since September 2025 I have been a research intern in the COSMO team at IBISC, funded by an IDEX Paris-Saclay scholarship, working on secure genomic data sharing that protects participants' identities.
I also lead the D4Gen Hackathon project on secure collection and transmission of electronic health records, which combines SDN-based medical IoT infrastructure with zero-knowledge smart contracts. Our team won the Shaker Genopole Challenge in 2026.

Outside research, I led the HUST Finance and Technology Club, organized the NestQuant 2023 and Chat'Innov AUF 2023 competitions, and ran francophone orientation events and workshops.
I speak English (C1, IELTS 7.0) and French (B2, DELF B2).
