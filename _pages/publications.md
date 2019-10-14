---
layout: page
permalink: /publications/
title: publications
description: 
years: [2019, 2018, 2017, 2016, 2015, 2013, 2012, 2010, 2009, 2008]
---

<h2 class="pub-type">Articles & Book Chapters</h2>
{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f articles -q @*[year={{y}}]* %}
{% endfor %}

<h2 class="pub-type">Conference Proceedings</h2>
{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f conf -q @*[year={{y}}]* %}
{% endfor %}

<h2 class="pub-type">Manuscripts in Preparation</h2>
  {% bibliography -f inprep %}

<h2 class="pub-type">Reports & Public Scholarship (Selected)</h2>
{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f reports -q @*[year={{y}}]* %}
{% endfor %}