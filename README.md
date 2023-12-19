# National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau

The project was done for a betting business'
![Purple Yellow White Modern Football Match Schedule Instagram Post](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/97ab8d83-5c45-4620-affb-fe956aea1d95)


## Table of Content
- [Introduction](#introduction)
- [Objective](#objective)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis)
- [The Dashboard](#the-dashboard)
- [Result and Findings](#result-and-findings)
- [Recommendation](#recommendation)



### Introduction

Football betting is a dynamic and thrilling aspect of the sports world, capturing the excitement of fans and enthusiasts worldwide. As fans watch their favorite teams compete on the field, the thrill of predicting match outcomes adds an extra layer of engagement. Football betting involves wagering on various aspects of the game, from predicting the winner to specific player performances or even the final score. 

With the rise of online platforms, football betting has become more accessible, offering fans the opportunity to immerse themselves in the sport on a whole new level. While it adds an element of suspense and entertainment, participants must approach football betting responsibly, emphasizing informed decisions and strategic thinking.

### Objective

- Trend of Winning Percentage for Home Teams Over Time
- Average Score Difference by Team Away
- Average Score Difference by Team Home
- Relationship Between Temperature and Humidity
- Number of Weekly Games Schedule by Stadium

### Data Source

Provided by the Company in CSV file format.

However, crucial research was done through other gaming websites and samples of other datasets. Here are some websites:

National Football League (NFL) game results since 1966 with betting odds information since 1979. The dataset was created from a variety of sources including games and scores from a variety of public websites such as ESPN, NFL.com, and Pro Football Reference. Weather information is from NOAA data with NFLweather.com as a good cross reference.  

Betting data was used from [Sun4cast](http://www.repole.com/sun4cast/data.htm) for the 1978-2013 seasons. 

[Pro-football](Pro-football-reference.com) data was then cross-referenced for betting lines and odds as well as weather data. 

From 2013 betting data reflects lines available at [sportsline](www.sportsline.com) and [aussportsbetting](aussportsbetting.com).

### Tools Used

- Microsoft Excel was used for cleaning and transformation.

- Tableau was used for Analysis, and reporting.

### Data Cleaning and Preparation

![Football Betting 1st Raw file](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/f4fd0544-72b8-4877-a1f7-36b495b95f31)
The source file

The dataset has about 14,870 rows and 13 columns with some of the column names as schedule_date,	schedule_season,	schedule_week,	schedule_playoff,	team_home,	score_home,	score_away,	team_away,	stadium	stadium_neutral, etc.

I did a thorough cleaning of the dataset by handling missing/null values, removing duplicates, and addressing any inconsistencies in the data.


![Ft ball betting After Transformation](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/c6f6f92c-246e-43bd-88ba-7b6aeeb86d9f)
After Cleaning

### Exploratory Data Analysis (EDA): 

- Correlation Analysis: I examine the correlation between different features and the target variable (game outcomes) to identify potential predictors within  the available table (columns)/
- Average Score Difference
- Winning Percentage for Home Teams
- Average Temperature
- Average Humidity
- Number of Games Played Each Week
- Trend of Winning Percentage for Home Teams Over Time
- Average Score Difference by Team Away
- Average Score Difference by Team Home
- Average Score Difference = SUM(ABS([score_home] - [score_away])) / COUNTD([schedule_date])
- Winning Percentage for Home Teams = SUM(IF [score_home] > [score_away] THEN 1 ELSE 0 END) / COUNTD([schedule_date])

### The Dashboard

![NFL Analysis](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/f7f3702c-a62b-482b-9677-0aea460619f3)


### Result and Findings

![Capture](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/69f544cf-5e71-4ee8-95d6-39d498ae8837)

Trend of Winning Percentage for Home Teams Over Time

- The chart depicts a declining trend in the winning percentage for home teams over time.
- The winning percentage was highest around 3.8% in the late '70s and has seen a consistent decline, reaching its lowest at approximately 2.143% projected for the year 2025.
- This trend is projected to continue, with the winning percentage for home teams continuing to decline.
- This data can be instrumental for betting analysis as it provides insights into the performance of home teams over time.
- However, it is important to note that this trend may not hold for every game, and other factors such as team performance, injuries, and weather conditions can also impact the outcome of games.


![Capture_1](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/90ec5372-8268-4477-9a7f-4a5eae1630c4)

Average Score Difference by Team Away

- The chart shows the average score difference by each NFL team when playing away games.
- The Baltimore Ravens have the highest average score difference, indicating their strong performance in away games.
- In contrast, the San Francisco 49ers have a significantly lower score difference, suggesting they may struggle more in away matches.
- Most teams hover around an average score difference of 13 to 19 points, indicating a general level of competitiveness in away games across the league.
- This data can be instrumental for betting analysis as it provides insights into each team’s performance and competitiveness during away games.


![Capture_2](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/28d71089-91e2-45a1-92ee-5a751ee87936)

Average Score Difference by Team Home

- The chart displays the average score difference by team home in football. Teams like the Baltimore Ravens, New England Patriots, and Kansas City Chiefs have a higher average score difference, indicating their strong performance at home games. On the other hand, teams like the Houston Texans and San Francisco 49ers have a lower average score difference when playing at home, suggesting they might not perform as well in their home games. The colorful bars represent different teams and are arranged in descending order of the average score difference. This data can be crucial for betting analysis as it provides insights into the teams’ performance patterns at home games.
- The Y-axis shows the average score differences ranging from -4 to 18.
- Teams are listed on the X-axis alphabetically; however, their bars are arranged based on the magnitude of their average score differences.
- A legend on the right side matches each team’s color to its name for easy identification.
- This data can be instrumental for betting analysis as it provides insights into each team’s performance and competitiveness during home games.


![Capture-4](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/96d11aa4-dbe9-480d-8767-fa81826533c0)

Number of Weekly Games Schedule by Stadium

- The chart displays the number of weekly games scheduled by various stadiums.
- Each stadium has a different number of games, ranging from 0 to 19.
- Some stadiums like “Arcisure Stadium” and “Alamo Dome” have more games scheduled (19 and 18 respectively), while others like “Franklin Field” and “Fratkin Field” have fewer (2 and 1 respectively).
- This data can be instrumental for betting analysis as it provides insights into the number of games scheduled at each stadium.
- However, it is important to note that this data may not hold for every season, and other factors such as team performance, injuries, and weather conditions can also impact the number of games scheduled at each stadium.


### Recommendation

- Based on the data presented in the charts, it appears that the Baltimore Ravens and Kansas City Chiefs have a higher average score difference when playing away games, indicating their strong performance in away games.
- On the other hand, teams like the Houston Texans and San Francisco 49ers have a lower average score difference when playing away games, suggesting they might not perform as well in their away games.
- This data can be instrumental for betting analysis as it provides insights into the teams’ performance patterns during away games. However, it is important to note that other factors such as team performance, injuries, and weather conditions can also impact the outcome of games.
















