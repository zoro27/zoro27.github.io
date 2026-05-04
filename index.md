---
layout: single
author_profile: true
title: "Welcome"
header:
  overlay_image: /assets/images/header-bg.jpg
  overlay_filter: 0.5
  caption: "Photo credit: [Unsplash](https://unsplash.com)"
  actions:
    - label: "📄 View My CV"
      url: /cv/
    - label: "📚 Publications"
      url: /publications/
---

## About Me

I am a **PhD candidate** at **McGill University** and **Mila — Quebec AI Institute**, working at the intersection of **systems neuroscience** and **artificial intelligence**.

---

## Research Interests

- **Systems Neuroscience** — Neural coding, population dynamics, brain-inspired computation
- **Artificial Intelligence** — Deep learning, representation learning, generative models
- **Neuroinformatics** — Tools and methods for large-scale neural data analysis

---

## News

<div class="news-list" markdown="1">

- **[Dec 2025]** New paper accepted in **Nature Communications** — "Latent brain subtypes of chronotype"!
- **[Jul 2025]** Our paper published in **Nature Human Behaviour** on the neurobiological underpinnings of chronotype.

</div>

---

## Recent Publications

{% assign sorted_pubs = site.publications | sort: "date" | reverse %}
{% for pub in sorted_pubs limit:3 %}
  <div class="pub-item" markdown="1">
  **[{{ pub.title }}]({{ pub.paperurl }})**  
  *{{ pub.authors }}*  
  **{{ pub.venue }}**, {{ pub.date | date: "%Y" }}{% if pub.volume %}, {{ pub.volume }}({{ pub.issue }}){% endif %}
  {% if pub.citation_count %} · Cited {{ pub.citation_count }} times{% endif %}
  </div>
{% endfor %}

[View all publications →](/publications/)

