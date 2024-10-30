---
layout: page
permalink: /publications/
title: publications
description: <a>*</a> denotes equal contribution.
years: [2024, 2023, 2022, 2020]
nav: true
nav_order: 3
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/fgm_wmc.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

<!-- _pages/publications.md -->

<div class="publications">

{% for y in page.years %}

  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
