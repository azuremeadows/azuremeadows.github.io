---
title: "Azure Meadows"
permalink: index.html
summary: This site contains information about Azure Meadows, a Hay Day neighborhood
nav_order: 1
last_modified_date: {{ site.github.pushed_at }}
---

# Welcome to Azure Meadows

Azure Meadows is a Hay Day Neighborhood (aka Guild, Clan, Alliance, Team, etc.).  This website has all of the rules and team norms for the neighborhood.

## Neighborhood Tags

<div class="code-example" markdown="1">
Fun
{: .label .label-yellow }

Active
{: .label .label-yellow }

Derby Focus
{: .label .label-yellow }

Derby: 320 Only
{: .label .label-yellow }

Helpers
{: .label .label-yellow }
</div>


## Neighborhood Stats

Derby information is based on the last four weeks.

- **Number of Members:** {{ site.data.memberStats | size }}
- **Derby League:** {{ site.data.neighborhoodStats[0]["Derby League"] | capitalize }}
- **Average Derby Placement:** {{ site.data.neighborhoodStats[0]["Average Derby Placement"] }}
- **Average Number of Derby Participants:** {{ site.data.neighborhoodStats[0]["Average Number of Derby Participants"] }}
- **Average Total Derby Points:** {{ site.data.neighborhoodStats[0]["Average Number of Points"] }}
- **Average Points per Player:** {{ site.data.neighborhoodStats[0]["Average Points per Player"] }}
- **Percentage of All Tasks Completed:** {{ site.data.neighborhoodStats[0]["Percentage of Tasks Completed"] }}%
