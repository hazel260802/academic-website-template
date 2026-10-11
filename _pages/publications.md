---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">
<h2>In Preparation</h2>

{% bibliography --query @unpublished %}

<h2>Conference, Workshop and Poster Papers</h2>

{% bibliography --query @inproceedings %}
</div>
