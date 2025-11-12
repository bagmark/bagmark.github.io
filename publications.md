---
layout: single
title: "Publications"
permalink: /publications/
---

Below is a curated list. See also my [Google Scholar](https://scholar.google.com/citations?user=-oZDUnQAAAAJ).

{% for p in site.data.publications %}
### {{ p.title }} ({{ p.year }})
**Authors:** {{ p.authors }}  
**Venue:** {{ p.venue }}

{% if p.abstract %}
**Abstract:** {{ p.abstract }}
{% endif %}

**Links:** 
{% if p.doi %}[DOI]({{ p.doi }}){% endif %}
{% if p.pdf %} · [PDF]({{ p.pdf }}){% endif %}
{% if p.code %} · [Code]({{ p.code }}){% endif %}
{% if p.slides %} · [Slides]({{ p.slides }}){% endif %}
{% if p.video %} · [Video]({{ p.video }}){% endif %}

---
{% endfor %}
