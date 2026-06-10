---
layout: default
title: Home
description: Learning design, AI literacy, and computing education portfolio of Sakshi Sharma.
---

<section class="hero">
  <div class="wrap hero-grid">
    <div>
      <p class="eyebrow">AI-enabled learning and computing education</p>
      <h1>Designing learning systems where pedagogy, data, and humane technology work together.</h1>
      <p class="lead">{{ site.data.profile.summary }}</p>
      <div class="hero-actions">
        <a class="btn" href="{{ '/resume/' | relative_url }}">Open linked resume</a>
        <a class="btn secondary" href="{{ '/projects/' | relative_url }}">Explore projects</a>
        <a class="btn secondary" href="{{ '/experience/' | relative_url }}">Experience details</a>
      </div>
      <div class="metric-strip">
        <div class="metric"><strong>9+</strong><span>years teaching and academic experience</span></div>
        <div class="metric"><strong>1000+</strong><span>faculty trained in AI literacy cohorts</span></div>
        <div class="metric"><strong>10</strong><span>publications and accepted research outputs</span></div>
        <div class="metric"><strong>5</strong><span>patent applications filed</span></div>
      </div>
    </div>
    <aside class="profile-panel">
      <img src="{{ site.data.profile.photo | relative_url }}" alt="Sakshi Sharma">
      <div class="profile-copy">
        <h2>{{ site.data.profile.name }}</h2>
        <p>{{ site.data.profile.headline }}</p>
        <p>{{ site.data.profile.current }}</p>
      </div>
    </aside>
  </div>
</section>

<section class="section">
  <div class="wrap">
    <div class="section-head">
      <div>
        <p class="eyebrow">Education technology strengths</p>
        <h2>Learning design strengths</h2>
        <p>My strongest fit is for roles that need learning design, faculty enablement, AI-enabled education workflows, and practical coordination across research, technology, and classroom use.</p>
      </div>
    </div>
    <div class="grid-3">
      <article class="card">
        <h3>Learning Experience Design</h3>
        <p>Designs lesson plans, activities, assessments, and feedback loops using student and faculty needs as the starting point.</p>
      </article>
      <article class="card">
        <h3>AI Literacy and Faculty Training</h3>
        <p>Developed and delivered AI literacy sessions for faculty development cohorts, with a focus on practical classroom adoption.</p>
      </article>
      <article class="card">
        <h3>Learning Analytics</h3>
        <p>Builds dashboard and classroom intelligence ideas that convert educational activity into useful signals for teachers and program teams.</p>
      </article>
    </div>
  </div>
</section>

<section class="section">
  <div class="wrap">
    <div class="section-head">
      <div>
        <p class="eyebrow">Selected work</p>
        <h2>Projects with deeper notes</h2>
      </div>
      <a class="btn secondary" href="{{ '/projects/' | relative_url }}">All projects</a>
    </div>
    <div class="grid-3">
      {% for project in site.data.projects %}
        <article class="card">
          <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
          <p>{{ project.short }}</p>
          <div class="tag-row">
            <span class="tag">{{ project.status }}</span>
          </div>
        </article>
      {% endfor %}
    </div>
  </div>
</section>

<section class="section">
  <div class="wrap">
    <div class="section-head">
      <div>
        <p class="eyebrow">Experience</p>
        <h2>Teaching, training, and academic coordination</h2>
      </div>
      <a class="btn secondary" href="{{ '/experience/' | relative_url }}">Detailed experience</a>
    </div>
    <div class="timeline">
      {% for item in site.data.experience %}
        <article class="timeline-item">
          <div class="period">{{ item.period }}</div>
          <div>
            <h3><a href="{{ item.url | relative_url }}">{{ item.role }}</a>, {{ item.organization }}</h3>
            <p>{{ item.summary }}</p>
          </div>
        </article>
      {% endfor %}
    </div>
  </div>
</section>
