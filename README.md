# Hearthstone-Webscraping
Hearthstone Web scraping Project.

Objective:

Scrap websites to retrieve necessary data to analyze and identify outliers in Hearthstone’s newest expansion for upcoming balance changes to improve player retention, increase daily users and community involvement.

Stakeholders: Members of Blizzard’s Hearthstone balancing team, content creators who are affiliated or create content around the game.

Data Collection:

Data is scraped in Python via Jupyter Notebooks ultizing BeautifulSoup and Selenium libraries. Scraping does not violate and terms and conditions as I will not be selling any collected data, all data scraped is public access and does not require a personalized login. Terms and conditions of sites scraped as well as laws in both Canada and the U.S were thoroughly investigated to ensure no violations were to be made. 

Tools Used:

  Jupyter Notebooks for Python web scraping and csv writing. 
  Microsoft Excel for importation of csv sheets and data cleaning.
  Tableau Public for visualizations and insights.


Python data gathering process and Excel data cleaning:

Had python write data into two different csv, one for each website. 
Follow link for detailed Python code base: https://github.com/adallan/Hearthstone-Webscrapping/blob/main/Hearthstone%20Webscraping.ipynb

Imported csv with ratings into a sheet then imported card statistics csv into the 2nd page of excel file. Duplicated ratings column since it contained both ratings and votes. Used Find&Replace to clean all columns and VLOOKUP to moved all statistical data over from the second sheet, making sure formula makes card names match up. Conditional formatting to highlight null value rows to remove as well as extra card name column. Data sets are imported into Tableau for visualization. 
Follow link to view the interactive dashboard: https://public.tableau.com/app/profile/alexander.allan/viz/HearthstoneExpansiondashboard/HearthstoneLatestExpansion

Insights and Recommendations:

To improve player logins, rententation and overall game balance I would recommend the following based on insights found from this project.

1) “Astalor Bloodsworn” is a incredibly popular card and is an extreme outlier in being most played, in the most decks, consistently above average win rate. All these indicate that it card quality is too high. I would recommend reducing its impact and sway on the game but not by extreme values as to keep it relevant.
2) “Shock spitter” and “Conjured Arrow” are both in the highest winrate deck currently in the game averaging at over 60% winrate. I would recommend changes in these cards to lessen their power which in turn will lower the win percentage of their deck. Any winrate over 55% can cause a danger to the game’s balance and in turn create negative player experiences or ‘feel bad’ moments.
3) Cards like “Light of the Phoniex”, “Flight of the Bronze” and  “Vexallus” are highly rated but preform poorly in play rates and deck win percentages. I recommend increasing card qualities for these and others that fall into the same filters to improve player logins and community involvement as it will encourage players to try new decks using these cards they previously had high hopes for before expansion launch.

For any further analysis I would run scrapping on card statistics every month for a year’s worth of expansions as well as gather login data to investigate insights into how balance changes affect the player base to quantify the value of these balance changes to the business as a whole.
