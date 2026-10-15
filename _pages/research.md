---
title: "Research"
permalink: /research/
---

<link rel="stylesheet" href="{{ '/assets/css/research.css' | relative_url }}">

<div class="research-page" markdown="1">

## Job Market Paper

{% for paper in site.data.research %}
{% if paper.group == 'jmp' %}{% include research-paper.html paper=paper %}{% endif %}
{% endfor %}

## Working Papers

{% for paper in site.data.research %}
{% if paper.group == 'working' %}{% include research-paper.html paper=paper %}{% endif %}
{% endfor %}

## Work in Progress

- **Pass-Through of Consumption Taxes under Political Pressure**  with [Sai Pitre](https://sai-pitre.github.io)

- **Digital Land and Property Improvement Tax Payment Mechanism in Malawi** (with [Klaus W. Deininger](https://scholar.google.com/citations?user=EthslK4AAAAJ&hl=en) and [Daniel Ayalew Ali](https://scholar.google.com/citations?user=NT2maDQAAAAJ&hl=en)) \
*[pre registered trial](https://www.socialscienceregistry.org/trials/19261)*

</div>
