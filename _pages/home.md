---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Semantic Web</a>
<a href="{{ '/research' | relative_url }}" class="chip">Knowledge &amp; Ontology Engineering</a>
<a href="{{ '/research' | relative_url }}" class="chip">Linked Data</a>
<a href="{{ '/research' | relative_url }}" class="chip">Enterprise Knowledge Graphs</a>
<a href="{{ '/research' | relative_url }}" class="chip">Artificial Intelligence</a>
<a href="{{ '/research' | relative_url }}" class="chip">Music Information Retrieval</a>
</div>

I work on connecting large language models with knowledge graphs. My research sits between the Semantic Web and AI: grounding LLMs in linked data to reduce hallucination, and making federations of SPARQL endpoints scale.

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

## About me

I am a postdoctoral researcher in the Wimmics team at Inria (Sophia Antipolis, France), where I build natural-language interfaces for secure federated querying over knowledge graphs, using GraphRAG to ground generated answers.

I completed my PhD in Computer Science at Nantes University (LS2N) in 2024, working on querying the Web as a knowledge graph: benchmarking and designing SPARQL federation engines, and evaluating LLMs for extracting Schema.org knowledge graphs from web pages. I then spent eighteen months at JusMundi in Paris, building knowledge-graph-based retrieval and fine-tuned embedding models for a legal Agentic RAG system.

I am based near Nice, France. Feel free to get in touch by [email](mailto:{{ site.email }}).
