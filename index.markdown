---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

[![Me](/assets/images/oberwolfach-me.jpeg "Copyright: Mathematisches Forschungsinstitut Oberwolfach")](https://opc.mfo.de/detail?photo_id=24560)

## About

Contact: [h.a.nieuwboer@uva.nl](mailto:h.a.nieuwboer@uva.nl)

I'm a PhD student at the [Korteweg-de Vries Institute](https://kdvi.uva.nl/) and [QuSoft](https://qusoft.org/) at the [University of Amsterdam](https://uva.nl/), advised by [prof. dr. Michael Walter](https://qi.ruhr-uni-bochum.de/walter) and [prof. dr. Eric Opdam](https://staff.fnwi.uva.nl/e.m.opdam/).
My office is located at [Centrum Wiskunde & Informatica](https://cwi.nl/).

I'm interested in classical and quantum algorithms for optimization problems with a lot of geometric or algebraic structure, such as (geodesic) convexity or having many symmetries. In particular, I'm interested in *scaling problems*, such as matrix scaling, operator scaling and tensor scaling. These problems have connections to representation theory, geometric invariant theory, quantum information theory, quantum many-body physics, machine learning, statistics, and numerical linear algebra.

## Papers
{% for item in site.data.papers %}
1. {{item.title}} \
  {{item.authors}} \
  {%- if item.published != nil -%} {%- for venue in item.published -%} {%- if venue.type == "arXiv" %}
  [{{venue.name}}:{{venue.data}}](https://arxiv.org/abs/{{venue.data}})
  {%- else if venue.type == "doi" %}
  [{{venue.name}}](https://dx.doi.org/{{venue.data}})
  {%- endif %}
  ({{venue.year}})
  {%- if forloop.index < forloop.length -%},{%- endif -%}
  {%- endfor %}{% endif %}
{% endfor %}

## Links
- [Google Scholar profile](https://scholar.google.com/citations?user=rD1Dw8kAAAAJ)
- [ORCID](https://orcid.org/0000-0003-3627-3636)
