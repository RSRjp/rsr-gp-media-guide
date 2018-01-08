---
layout: single
title: "日程"
permalink: /races/
header:
  overlay_image: /assets/images/races_idx.jpg
---

{% for race in site.data.races %}
## <i class="fa fa-calendar-alt" aria-hidden="true"></i> {{ race.date | date:'%Y/%m/%d' }}
<i class="fa fa-flag-checkered" aria-hidden="true"></i> 第{{ forloop.index }}戦: {{ race.name }}
: <i class="fa fa-globe" aria-hidden="true"></i> {{ race.location }} - {{ race.circuit.name }}
{% endfor %}
