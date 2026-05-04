---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

## Selected Publications

{% assign sorted_pubs = site.publications | sort: "date" | reverse %}

{% for pub in sorted_pubs %}
<div class="publication-card" markdown="1">

### {{ pub.title }}

**{{ pub.authors }}**

*{{ pub.venue }}{% if pub.volume %}, {{ pub.volume }}({{ pub.issue }}){% endif %}{% if pub.pages %}, pp. {{ pub.pages }}{% endif %}{% if pub.date %}, {{ pub.date | date: "%Y" }}{% endif %}*
{% if pub.citation_count %} · Cited {{ pub.citation_count }} times{% endif %}

{{ pub.excerpt }}

{% if pub.paperurl %}[📄 Paper]({{ pub.paperurl }}){: .btn .btn--small .btn--primary}{% endif %}
{% if pub.codeurl %}[💻 Code]({{ pub.codeurl }}){: .btn .btn--small}{% endif %}
{% if pub.slidesurl %}[📊 Slides]({{ pub.slidesurl }}){: .btn .btn--small}{% endif %}

</div>

{% endfor %}
