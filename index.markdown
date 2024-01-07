---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

[![Me](/assets/images/oberwolfach-me.jpeg "Copyright: Mathematisches Forschungsinstitut Oberwolfach")](https://opc.mfo.de/detail?photo_id=24560)

## About

Contact: [hani@math.ku.dk](mailto:hani@math.ku.dk) (previous e-mail address: [h.a.nieuwboer@uva.nl](mailto:h.a.nieuwboer@uva.nl), may become inactive soon)

I am currently a postdoctoral researcher at [QMATH](https://qmath.ku.dk) at the [University of Copenhagen](https://ku.dk/), advised by [prof. dr. Matthias Christandl](https://www.math.ku.dk/english/staff/?pure=en/persons/475476) and [dr. Laura Mančinska](https://www.math.ku.dk/english/staff/?pure=en/persons/604782).
Formerly, I was a PhD student at the [Korteweg-de Vries Institute](https://kdvi.uva.nl/) and [QuSoft](https://qusoft.org/) at the [University of Amsterdam](https://uva.nl/), and an affiliated researcher at the [Ruhr-Universit&auml;t Bochum](https://www.ruhr-uni-bochum.de/), advised by [prof. dr. Michael Walter](https://qi.ruhr-uni-bochum.de/walter) and [prof. dr. Eric Opdam](https://staff.fnwi.uva.nl/e.m.opdam/).

I'm interested in classical and quantum algorithms for optimization problems with a lot of geometric or algebraic structure, such as (geodesic) convexity or having many symmetries. In particular, I have worked on *scaling problems*, such as matrix scaling, operator scaling and tensor scaling. These problems have connections to representation theory, geometric invariant theory, quantum information theory, quantum many-body physics, machine learning, statistics, and numerical linear algebra.

## Papers
{% for item in site.data.papers %}
1. {{item.title}} \
  {{item.authors}} \
  {%- if item.published != nil -%} {%- for venue in item.published -%} {%- if venue.type == "arXiv" %}
  [{{venue.name}}:{{venue.data}}](https://arxiv.org/abs/{{venue.data}})
  {%- elsif venue.type == "doi" %}
  [{{venue.name}}](https://dx.doi.org/{{venue.data}})
  {%- elsif venue.type == "other" %}
  [{{venue.name}}]({{venue.data}})
  {%- endif %}
  ({{venue.year}})
  {%- if forloop.index < forloop.length -%},{%- endif -%}
  {%- endfor %}{% endif %}
{% endfor %}

## Links
- [Google Scholar profile](https://scholar.google.com/citations?user=rD1Dw8kAAAAJ)
- [ORCID](https://orcid.org/0000-0003-3627-3636)
