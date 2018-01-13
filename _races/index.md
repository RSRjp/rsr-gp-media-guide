---
layout: single
title: "日程"
permalink: /races/
header:
  overlay_image: /assets/images/races_idx.jpg
---

全てのレースは日本時間 22:00 よりサーバーオープン、22:30 より予選セッション(15分)開始となります。
{: .notice-info }

{% for race in site.data.races %}
## <i class="fa fa-calendar-alt" aria-hidden="true"></i> {{ race.date | date:'%Y/%m/%d' }}
<i class="fa fa-flag-checkered" aria-hidden="true"></i> 第{{ forloop.index }}戦: {{ race.name }}
: <i class="fa fa-globe" aria-hidden="true"></i> {% include ja_name name=race.location %} - {{ race.circuit.name }}
{% endfor %}
