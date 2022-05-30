---
title: Member Stats
permalink: member-stats.html
nav_order: 2
---

Derby information is based on the last four completed derbies.  Strikes are removed after {{ site.data.neighborhoodStats[0]["Strike Expiration Delay"] | pluralize: 'day', 'days' }}.

Information last updated on {{ "now" | date: "%Y-%m-%d %H:%M %Z" }} UTC

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

## Notes

Join dates above may be estimations.  Members with a join date of 4/1/2022 have been members before this information was ever recorded.
