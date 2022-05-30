---
title: Member Stats
permalink: member-stats.html
nav_order: 2
---

Derby information is based on the last four weeks.  Strikes are removed after 60 days.

Information last updated on {{ "now" | date: "%Y-%m-%d %H:%M" }}

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
