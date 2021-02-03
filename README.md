# Sports-Records-Bot
Have you ever heard an announcer say “He was their winningest coach” and wondered if that was actually true? If you have then, this automation is for you. This automation will send you an email showing the records of teams under different head coaches. Showing you who actually is the winningest head coach whether you want to see it for individual teams or leaguewide.
This automation measure winningest in a few different ways including: wins per year, wins per game, postseason wins per postseason games, divisional championships, and national championships.

This automation uses UiPath. It has implemented Studio, Orchestrator, and Assistant. This automation uses the REFramework template UiPath provides. It incorporates Ui interactions, excel automation, and email automation. It also uses form activity along with JSON parsing and many switch statements to provide the ability to get these calculations for multiple sports, multiple sheets, and sorted however the user wants.

Sports this automation supports include: college football (NCAAF CFB), NHL, and NFL. Support for MLB and NFL are waiting to be added soon. This automation can be expanded upon in future iterations as some of the same workflow files are used by all sports and switch statements can have more cases added to.

Some limitations of this project include:
- No conference championships for CFB readily available.
- NFL website only gives last name of coaches.
- Only adds last coach of team in a season.
- Does not split up championships based on coach conference/division team trio only coach team pair.
- First CFB national championships does not always list coach.
- Some CFB does not list coach.
- Can run multiple leagues at a time properly only if running only league pages.
- Can only run 1 coach or team at a time.

## Worksheets
There are 3 worksheets that may be contained in the workbook you receive via the email attachment. Each sheet for each league contains the columns:
- Team name
- Coach name
- Years/seasons as coach
- Wins
- Losses
- Games
- Postseasons reached/games is equivalent for CFB
- National championships
- Wins per year
- Wins per game
- Postseason appearances per year


NFL contains the additional columns:
- Conference championships

CFB contains the additional columns:
- Postseason wins

NHL contains the additional columns:
- Division
- Conference
- Postseason wins
- Postseason games
- Postseason wins per year
- Conference championships


The individual worksheets contain more columns on top of the ones listed above. The differences between the pages are:
1. League specific page:
    - Sheet named league name user selects from form.
2. Team specific page:
    - Sheet named team name user inputs into form.
3. Coach specific page:
    - Sheet named coach name user inputs into form.
    - If applicable can have multiple rows with different teams as coaches change jobs.

## Flowchart
![Flowchart](https://github.com/nfh2019/Sports-Records-Bot/blob/master/SportsRecords.png)
