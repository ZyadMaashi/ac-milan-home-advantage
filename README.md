# ac-milan-home-advantage
Data analysis in Python of 21 Serie A seasons from 05/06 to 25/26 testing if AC Milan's home advantage is larger than other Serie A teams'.

# Does AC Milan Have a Larger Home Advantage Compared to Other Serie A Teams?

 I've been an AC Milan fan my entire life, so I wanted to see if Milan benefits more by playing at home comparted to other teams. I measured home advantage by making home and away points per game separate and subtracting them.

## Data
The Serie A Match results are from football-data.co.uk for 21 seasons (05/06 to 25/26): 7,980 matches after removing the 5 empty rows. The notebook downloads the data directly.

## Main findings
- Milan's points per gap is 0.34, placing them at 17th out of 20 and the league median is 0.43.
- Milan's 95% range of values which is 0.16 to 0.52, includes the league median, so there isn't any real difference between Milan and other teams.
- The league-wide home advantage fell from 0.69 (05/06 to 09/10) to 0.22 (19/20 to 25/26).
- In The last seven seasons Milan's gap was almost zero by being -0.04, but the interval was wide and I can't rule out the chance of luck.

## Method
Data cleaning, the points-per-game gap, bootstrap resampling (10,000 draws), season by season comparison by the league gap.

## Limitations
- I only used goals and results. There weren't any attendance data in the files, so I wasn't able to test the Covid years that had no attendance.
- The last seven seasons window was chosen after looking at the chart, so this isn't a planned test it; was an exploratory check.

 ## How to run
 1. Open 'ac_milan_home_advantage.ipynb' in Google Colab
 2. Click Run all.
 3. An internet connection is required for the notebook to download the data.
