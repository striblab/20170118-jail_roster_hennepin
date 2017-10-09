Star Tribune - Hennepin County Jail Roster
================

by [Frey Hargarten](https://github.com/jeffhargarten)

The Google Sheet and associated Google Script can automatically or manually pull and archive the most recent [Hennepin County jail roster](https://www4.co.hennepin.mn.us/webbooking/resultbyname.asp). It also checks the roster against a provided list of names and highlights whenever one of those names is in custody.

Use the following steps to set it up:

1. Import the roster.xlsx to Google Sheets

2. In Google Sheets, click Tools > Script editor...

3. Copy and paste the contents of scraper.js into the Script Editor

4. Name, save and grant access to the script

5. Refresh the Google Sheet. A menu item called JailRoster will appear

6. To run the script manually, click JailRoster > Refresh

7. To run it automatically, setup a trigger in the Google script for the chronTasks() function and set the interval

8. Edit the names you want to check for in the 'names' tab

9. All roster scrapes will be stored and timestamped in their own tabs

10. Found names will be marked with the name of the tab they last appeared