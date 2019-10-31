---
layout: page
permalink: /publications/
title: Publications
description: star* denotes equal contribution.
years: [2020,2019]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
