---
title: Derby Performance History
parent: Derbies
nav_order: 3
---

Derby information is based on the last four weeks.

<table>
  {% for row in site.data.DerbyHistory %}
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
