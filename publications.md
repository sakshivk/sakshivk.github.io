---
layout: page
title: Publications
permalink: /publications/
eyebrow: Research outputs
intro: Publications and accepted research outputs across blockchain, cyber security, deep learning, healthcare records, and education technology.
---

{% assign grouped = site.data.publications | group_by: "year" | sort: "name" | reverse %}
{% for group in grouped %}
## {{ group.name }}

{% for paper in group.items %}
<article class="card" id="{{ paper.anchor }}">
  <h3>{{ paper.title }}</h3>
  <p>{{ paper.venue }}</p>
</article>
{% endfor %}
{% endfor %}

## Research Themes

- Computing education and technology-supported teaching.
- Blockchain systems for security, auditability, and healthcare records.
- Cyber security and cloud computing.
- Deep learning applications in emotion recognition and biomedical classification.
