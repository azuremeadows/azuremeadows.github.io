---
title: Derby Performance History
parent: Derbies
nav_order: 90
---

Derby information is based on the last four completed derbies.

Information last updated on {{ "now" | date: "%Y-%m-%d %H:%M %Z" }}

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
