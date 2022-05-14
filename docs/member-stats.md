---
title: Member Stats
permalink: member-stats.html
nav_order: 2
---

Please note that these numbers are not real and are only provided for testing purposes. 😀

<table>
  {% for row in site.data.memberStats %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
