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

*{{ pub.venue }}{% if pub.date %}, {{ pub.date | date: "%B %Y" }}{% endif %}*

{{ pub.excerpt }}

{% if pub.paperurl %}[📄 Paper]({{ pub.paperurl }}){% endif %}
{% if pub.codeurl %}[💻 Code]({{ pub.codeurl }}){% endif %}
{% if pub.slidesurl %}[📊 Slides]({{ pub.slidesurl }}){% endif %}
{% if pub.posterurl %}[🖼️ Poster]({{ pub.posterurl }}){% endif %}

</div>

---

{% endfor %}
