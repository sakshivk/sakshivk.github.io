---
layout: page
title: Experience
permalink: /experience/
eyebrow: Teaching and design practice
intro: Experience details prepared for direct linking from a concise resume.
---

{% for item in site.data.experience %}
<article class="card" id="{{ item.anchor }}">
  <h2>{{ item.role }}</h2>
  <p><strong>{{ item.organization }}</strong> | {{ item.period }}</p>
  <p>{{ item.summary }}</p>
  <div class="tag-row">
    {% for tag in item.tags %}
      <span class="tag">{{ tag }}</span>
    {% endfor %}
  </div>
  <ul>
    {% for point in item.highlights %}
      <li>{{ point }}</li>
    {% endfor %}
  </ul>
</article>
{% endfor %}

## Guest Lectures and Outreach

Delivered guest lectures under the Integrated Scheme for School Education in Himachal Pradesh government schools on Python, web development, and computer networks for students from grades 9 to 12. Schools included GSSS Shahpur, GSSS Amni, GSSS Baroh, GSSS Pauria, GSSS Deha, GSSS Jeori, GSSS Nankhari, GSSS Matal, and GSSS Sarotri.
