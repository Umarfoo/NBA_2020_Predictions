# Important Links

Link to the original [project repository.](https://github.com/Mirgadir/Project1)

# NBA 2020 Winners/Losers Predictions

### PROJECT BACKGROUND
It all started when a group of 5 hotshots were hired by Mr. Drake Romaro, a billionaire who made his fortune from betting on sports. While his initial bets were lucky hoops, which made him a fortune, now he thinks he needs to develop a calculated winning strategy.

Mr. Romaro has started his own analytics company to analyze the 2019 – 2020 basketball season data to predict the winning team. He has recently asked fresh graduates from UT Austin Data Camp to help him win big this season.

### QUESTIONS TO ANSWER
1. Which are the top 8 teams for each conference in the current season, till the last data point? What are the scores of the top 8 teams? And their win to loss ratio. For each conference.
2. Does the home team win more or the visitors team win more matches?
3. What are the locations of the game? Heat map indicators of teams with more wins.
4. Calculating correlation between team player stats, team field goal % and other variables against games won by the team.
5. Defining winning parameters to determine a score for “Win Factor” of each team.

### BREAKDOWN OF TASKS
- Importing and merging relevant data files.
- Create data frame of top 8 teams and their respective win/loss scores and ratio.
- Make a bar graph with wins in green and losses in red.
- Calculate the number of win counts by home team and visitors team, and represent them in a pie chart.
- Use Google API to match venue location and extract their latitude and longitude. Map game location on Google Maps.
- Heat map indicators of teams with more wins percentage.
- Extract player points and average their data in new data frame. Sum all the team’s player data and match them to their respective team.
- Calculating correlation between team player stats and game won by the team.
- Make scatter plots of Team Win vs. Player Stats and other variables and run regression for each conference to find relationship between variables.
- Make observation as per analysis results and define winning parameters for win prediction.

## Conclusion/Recommendations
Q.1. Who are the top 8 teams for East and West Conference?
Ans. To find the top eight teams, we looked at the win loss ratio of all the teams and found the top 8 teams for both the Eastern and Western conference.

Q.2. Does the home team win more matches or the visitor team?
Ans. We found by looking at the 2019-2020 season data, that there is a noticeable advantage to playing on a team’s home court. Using the 971 games played for the season for reference, the home team won 55.1% of the time.

Q.3. Where are the locations of the game?
Ans. Using google places API, we used a location search for each arena based on the ones listed in the data sets acquired from the Sports Feeds API to then map them across the united states. We then used these points and the teams win percentages as the factor for our heat map layer.

Q.4. How can we determine who has the best chance of winning?
Ans. Answering this question took some crunching, but we were able to synthesize a team’s win factor by looking at a multitude of factors ultimately leading to a team’s success. We found our data using the Sports Feeds API to get the most up to date data. First, we looked at their win percentage, then we looked at how many players on a team’s roster scored over 900 pts total as our threshold. Then after running linear regressions on Field Goal Totals, Points Difference, Average Points Scored, and Final Player Efficiency Rating, we were able to devise a formula for getting a teams Win Factor. Using the slope of these individual regressions as a multiplier for the top teams, we came up with the formula to make our final recommendations.

Q.5. Who had the best chance of winning?
Ans. From our findings and analysis of the 2019-20 season data, the Bucks, Lakers, and the Clippers had the best chance of winning at the conclusion of the season should it not have been cancelled due to COVID-19. This was based on their Win Factor which can be seen against the other teams in the bar graph titled “East vs West! Who Will Win?”
