---
title: Activity Spreadsheet
parent: Elder Info
nav_order: 1
---

Members who are elders, co-leaders, or a leader, have access to the spreadsheet that records activity for the neighbhorhood.  It provides a lot of the data that this site relies upon and makes it easy for everyone to understand where their place is.

This spreadsheet is relatively easy, especially if you have Google Sheets (or Excel) experience.  Most of the complexity has been made in other spreadsheets where non-experienced people won't mess anything up.

The link to the Activity Spreadsheet has been pinned in the Discord channel.

# Overview

The spreadsheet has a lot of spreadsheets but don't worry: you'll only be messing with 3 of these at the most.

* Activity Tracker: Tracks farm activity as a way to test if a player is still active
* Derby Participation: Tracks participation for players who opt into the derby
* Neighbors: Tracks players in the neighborhood

## Activity Tracker

The Activity Tracker is a flat spreadsheet that has a listing of members that were in the neighborhood at the time that activity was recorded.  There are 5 columns:

* Date
* Neighbor
* Activity Type
* Points (This value is not used at this time)
* Notes

*Generally speaking*, activities that can be completed quickly are worth higher points because it means that the player has played the game in the last hour or so.  For example, growing anything that matures within an hour is worth 60 points with full derby participation is worth 100 points.

### Completing an Activity Check

1. Record the date that you are performing the check in Column A.
1. For Columns B and C, you should notice that there is a dropdown available.  It's much easier to go through the neighborhood member listing than it is to copy and paste from the spreadsheet.  That's because it's often easier to go in order up and down the list than it is to hunt and peck.  As a result, in the game, click on the neighborhood house and record each member's name from top to bottom.
1. **Now the hard part:** Check each neighbor for activity.  Click on each neighbor and try to find the highest-point activity.  Start by giving each member who has participated in the last derby with a participation check.  After that, remember that crops must be in the process of growing (not fully mature), livestock should be walking around (not ready to be gathered), etc.
1. Repeat the process for each member, only marking their farm as inactive if you cannot find any sign of activity.  Some common long-term activities to check: Jam Maker and Smelters are often working for players that may be sleeping overnight.
1. Once you are complete, record members who you marked as "inactive" and report it in the "Activity Tracking" discord channel.

## Derby Participation

Derby Participation, much like the Activity Check, is a flat table with 8 columns.  Some of the fields will be filled by formulas.

* Date
* Derby Type: Auto-populated by formula
* Neighbor
* Tasks Completed
* Tasks Assigned
* Points
* Extra Task Taken
* Points per Task: Auto-populated by formula

### Recording Derby Participation

**It is important to enter the Derby Participation information before 2300 UTC Mondays as the website pulls the information from the spreadsheet at that time.**

1. Record the date that the derby began.  The date should always be a TUESDAY.
1. Skip column B for now.
1. For Column C, you should notice that there is a dropdown available.  It's much easier to go through the derby score board and type each participant in their own row for this column.
1. For each derby participant, record how many tasks they completed into Column D, how many tasks they were assigned into Column E, the number of points scored into Column F, and if they took an extra task into Column G.  
1. Column H is a formula that you can drag from the previous row down to the rest of the rows.  To do so, click on the row above the blank one and use your computer's "Copy" function.  For Mac, this is ⌘-C; for Windows, this is Ctrl-C.  Then use your computer's paste function for all of the rows that are blank for each player in the current derby.
  * Depending on the derby, any members with an average points per task less than 320.0 should receive a strike.

For Column B, you'll need to enter the Derby type in `Derby History`.  Click on this spreadsheet and you'll a table with 9 columns.  Many of these columns are auto-populated by formula.  You only need to worry about three columns:

* Starting Date
* Type
* Place

If there is a row for the current derby date, edit the columns as necessary.  If there isn't, add the starting date of the derby into Column A, the type of derby in Column B, and what place the neighborhood got in Column D.

All other columns are completed by formulas so you may copy the cell information from other populated rows down the sheet.

The derby type is a Drop Down to prevent bad data entry.  If you need to add a new Derby Type, you can do so in Column F of the `VLOOKUP` spreadsheet.  This spreadsheet is very complex and it is recommended that you only do this if you are comfortable doing so.

Once the Derby History has been entered, return to the `Derby Participation` spreadsheet and copy the formula from another row's Column B down all the blank rows for the current Derby.

