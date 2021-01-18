# Sports-Records-Bot
Have you ever heard an announcer say “He was their winningest coach” and wondered if that was actually true? If you have then, this automation is for you. This automation will send you an email showing the records of teams under different head coaches. Showing you who actually is the winningest head coach whether you want to see it for individual teams or leaguewide.
This automation measure winningest in a few different ways including: wins per year, wins per game, postseason wins per postseason games, divisional championships, and national championships.


This automation uses UiPath. It has implemented Studio, Orchestrator, and Assistant. This automation consists of 3 different workflow projects each using a different template. Sports_Records_Main uses Orchestration Process template, Sports_Records_Calculations uses the Background Process template, and Sports_Records_Data uses a blank Process.
Sports_Records_Main implements both of the other projects and uses a Form Task activity.

## Worksheets
There are 3 worksheets that may be contained in the workbook you receive via the email attachment. Each sheet contains the columns:
- Division
- Years
- Wins
- Losses
- Games
- Postseason wins
- Postseason games
- Divisional championships
- National championships

The individual worksheets contain more columns on top of the ones listed above. The differences between the pages are:
1. League specific page:
    - Sheet named league name user selects from form.
    - Also contains both team and head coach names.
2. Team specific page:
    - Sheet named team name user inputs into form.
    - Also contains coach name.
3. Coach specific page:
    - Sheet named coach name user inputs into form.
    - Also contains team name.
    - If applicable can have multiple rows with different teams as coaches change jobs.

## Flowchart
![Flowchart](https://github.com/nfh2019/Sports-Records-Bot/new/master?readme=1/SportsRecordsFlowchart.png)
