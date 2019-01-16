# RankingsDateScraper
Rankings Date Scraper to Extract Date Information from rankings.the-elite.net

Files:
Funcs.py - Contains functions to open file, open webpage, and parse the xml of rankings.the-elite.net
RankingsDataScraper.py - Run the functions in Funcs.py, change variables here to get desired results
out/60 GEPD Finished.xlsx - Excel file which contains the data and pivot table

Current Version Data gathered - 12/12/2018 - 12/13/2018 (Goldeneye), 12/14/2018 (Perfect Dark)

Current Use, in rankingsdatascraper.py
  edit high-points for upper bound of points info to scrape data, edit low points for lower bound of points info to scrape data
  e.g. high-points, low-points = 100, 60 -- will scrape all rankings data for personal bests between 100 and 60 points for the specified level

  edit select_a, select_sa, select_00a to determine which difficulties to scrape data from
  e.g. True, False, True - Will scrape data from agent and 00agent(perfect agent if game is perfect-dark)
  
  edit game to determine game, level to determine level
  e.g. goldeneye, aztec will scrape data from aztec; perfect-dark, defection will scrape data from defection

  edit filename to change the file that scraped data will be written to
  current use case is to write to a .csv and copy/paste manually into a .xlsx for data analysis
  
  current excel file in Program_Files/Out - 60 GEPD Finished.xlsx contains data for all personal best times worth 60 or more points, instructions for pivot table use contained
  main data analysis tools in the chart worksheets
  can filter by level, year, time, points, name, etc. as well as filter dates by quarters or months using the timeline below the chart
  main usage for the moment is to filter by level, as the chart contains information for all current personal-best times worth above 60 points on all levels
