---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Semantic Web</a>
<a href="{{ '/research' | relative_url }}" class="chip">Knowledge / Ontology Engineering</a>
<a href="{{ '/research' | relative_url }}" class="chip">Linked Data</a>
<a href="{{ '/research' | relative_url }}" class="chip">Enterprise Knowledge Graphs</a>
<a href="{{ '/research' | relative_url }}" class="chip">Artificial Intelligence</a>
<a href="{{ '/research' | relative_url }}" class="chip">Music Information Retrieval</a>
</div>

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}
