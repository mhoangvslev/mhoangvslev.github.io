---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">
<h2>Refereed Journal Articles</h2>

{% bibliography --query @article %}

<h2>Refereed Conference Proceedings</h2>

{% bibliography --query @inproceedings %}

<h2>Thesis</h2>

{% bibliography --query @phdthesis %}

<h2>Other</h2>

{% bibliography --query @misc %}

{% bibliography --query @techreport %}
</div>
