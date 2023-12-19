# National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau

The project was done for a betting business'
![Purple Yellow White Modern Football Match Schedule Instagram Post](https://github.com/Solution92/National-Football-League-Scores-and-Betting-Analysis-with-Excel-Tableau/assets/144762124/97ab8d83-5c45-4620-affb-fe956aea1d95)

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

























