---
layout: page
permalink: /publications/
title: publications
description: Selected publications.
years: [2018,
2016,
2014,
2013,
2012,
2011,
2010,
2009,
2008,
2007,
2006,
2005
2002,
1997,
1996,
1995,
1994,
1992,
1985,
1979
]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
