---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Time-Sensitive Networking</a>
<a href="{{ '/research' | relative_url }}" class="chip">Network Calculus</a>
<a href="{{ '/research' | relative_url }}" class="chip">Dynamic Reconfiguration</a>
<a href="{{ '/research' | relative_url }}" class="chip">Blockchain</a>
<a href="{{ '/research' | relative_url }}" class="chip">Zero-Knowledge Proofs</a>
<a href="{{ '/research' | relative_url }}" class="chip">Privacy-Preserving Systems</a>
<a href="{{ '/research' | relative_url }}" class="chip">IoT &amp; SDN</a>
</div>

I'm currently a PhD candidate in Computer Systems Networking and Telecommunications at the [Conservatoire national des arts et métiers (Cnam)](https://www.cnam.fr/) and [ECE Engineering School](https://www.ece.fr/) in Paris, within the [LyRIDS](https://www.ece.fr/en/research-focuses-and-structuring) (ECE) and [CEDRIC](https://cedric.cnam.fr/) (Cnam) laboratories and the SMI doctoral school.
My current research focuses on [Time-Sensitive Networking (TSN)](https://1.ieee802.org/tsn/), deterministic [network calculus](https://en.wikipedia.org/wiki/Network_calculus) and the certified dynamic reconfiguration of TSN networks, as well as blockchain, [zero-knowledge proofs](https://en.wikipedia.org/wiki/Zero-knowledge_proof) and privacy-preserving systems for healthcare and genomic data.

<div class="callout callout-success" markdown="0">
<div class="callout-title">{% include icon.html name="award" class="callout-icon" %} Network calculus notes</div>
<p>I am writing a learning series on network calculus applied to TSN, from worst-case bounds to dynamic reconfiguration. Start with <a href="https://cnam-ece.github.io/learning-materials/blog/why-deterministic-guarantees" target="_blank" rel="noopener">Why deterministic guarantees? From TSN to worst-case bounds</a>, or browse the code on <a href="https://github.com/CNAM-ECE" target="_blank" rel="noopener">GitHub</a>.</p>
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

Since November 2026, I have been preparing a PhD at Cnam and ECE on the certified dynamic reconfiguration of TSN networks, which aims to keep provable worst-case latency guarantees while a network is reconfigured at runtime.
I hold a Master 2 in Computer Networks (Network Systems track, CNS-SR) from Université d'Évry Paris-Saclay (2026), and an engineering degree in Computer Science from the PFIEV elite programme at Hanoi University of Science and Technology (HUST, 2024).

My research experience started at HUST's BKCS lab, where I worked with Prof. Tran Hai-Anh on multi-objective deep reinforcement learning for edge-cloud server selection, published at IEEE Cloud Summit 2024.
In 2025, I did a 3-month research internship at Universidade do Porto (FEUP), funded by Erasmus+ and IDEX Paris-Saclay, on context-aware location privacy for multimodal transportation with Prof. Mariana Cunha and Prof. João P. Vilela (JDSE 2025).
From September 2025, I was a Master 2 research intern in the COSMO team at the IBISC Laboratory under Prof. Nazim Agoulmine, working on blockchain-based genomic data sharing with zero-knowledge proofs. This work was published at ADVANCEs 2026 and presented as posters at the P3S3 Summer School and [ACM womENcourage 2026](https://womencourage.acm.org/2026/index.php/poster-session/).
I also led the D4Gen Hackathon project on secure collection and transmission of electronic health records over [Software-Defined Networks](https://en.wikipedia.org/wiki/Software-defined_networking) emulated in [Mininet-WiFi](https://mininet-wifi.github.io/), whose team won the [Shaker Genopole Challenge](https://genopole.agorize.com/web/en/challenges/618/teams/2643/participation), and co-authored [LLMThings](https://llmthings.github.io/demo/), which received the [Best Presentation Award](https://www.ibisc.univ-evry.fr/anais-sadoudi-et-huyen-trang-le-recoivent-le-best-presentation-award-a-la-jdse-2026-english-version-below/) at [JDSE 2026](https://jdse2026.github.io/program/).

Beyond research, I was President of the HUST Finance and Technology Club, where I organized more than 10 workshops and events on blockchain and crypto-finance for 70 members, and led the extracurricular activities committee of the HUST Francophone Club.
I organized the NestQuant 2023 and Chat'Innov AUF 2023 programming competitions, which brought together more than 150 participants, as well as francophone career orientation events.
I also served as a StartupCity ambassador and represented BK Fintech at the Korea–Vietnam Entrepreneurship Education Forum.
