---
layout: page
title: Projects
permalink: /projects/
eyebrow: Design and technology work
intro: Detailed project notes for resume links, including learning analytics, classroom intelligence, student-facing learning resources, and education technology prototypes.
---

{% for project in site.data.projects %}
<article class="card" id="{{ project.anchor }}">
  <h2>{{ project.title }}</h2>
  <p><strong>Timeline:</strong> {{ project.timeline }} | <strong>Status:</strong> {{ project.status }} | <strong>Stack/focus:</strong> {{ project.stack }}</p>
  <p>{{ project.short }}</p>
  <ul>
    {% for detail in project.details %}
      <li>{{ detail }}</li>
    {% endfor %}
  </ul>
</article>
{% endfor %}

## Research and Product Direction

The projects are connected by a common design question: how can teachers and academic teams receive useful signals without increasing their workload? The technology is designed around lesson flow, learner motivation, assessment, and instructor decision-making.

## Useful Resume Links

- [Spurti](#spurti)
- [Spandan](#spandan)
- [Student Learning Resources](#student-learning-resources)
