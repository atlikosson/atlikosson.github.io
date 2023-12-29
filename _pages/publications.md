---
layout: page
permalink: /publications/
title: publications
description: <span>*</span> denotes equal contribution
nav: true
nav_order: 2
years: [2024, 2023, 2021, 2020, 2019]
---
<!-- _pages/publications.md -->
<div class="publications">
    {% for y in page.years %}
    <div class="bibliography-sep row p-0 mb-2">
        <div class="col-sm-11 p-0">
        {% bibliography -f papers -q @*[year={{y}}]* %}
        </div>
        <div class="col-sm-1 align-self-end mt-2 p-0 pr-1">
        <h3 class="bibliography-year">{{y}}</h3>
        </div>
    </div>
    {% endfor %}
</div>
