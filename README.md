Project4
Data set used: https://github.com/fivethirtyeight/data/tree/master/soccer-spi
This dataset contains predictions about club soccer predictions. Spi_matches.csv contains data of various leagues from 2016 to 2020. It contains the data of all teams, matches played, and goals scored. Three metrics have been used to evaluate team’s performance after each match. Adjusted goals, shot-based expected goals (xg) and non-shot expected goals(nsxg) are the three metrics used to predict the goals scored by each team. spi_global_rankings.csv dataset contains global ranking of 618 soccer teams and soccer power index (SPI) across the globe.

1.	Data Cleaning
    Loaded the spi_matches.csv and spi_global_rankings.csv using pandas library
    
    Performed data cleaning in soccer data and removed the redundant records and null records and described the dataset
    
2.	Data Transformation

    Using dimentionality reduction, created a dataframe consisting of only the columns required for data analysis

    Dropped the columns previous rank and league from global ranking data
    
    Replaced in ‘Nan’ values with mean value of the column in the data set for the columns xg, nsxg and adj_score
    
    Merged 'spi_matches' and 'spi_global_rankings' dataframe on team name in a single dataframe in order to get entire dataset in one frame.

3.	Data Analysis
	Analyzed the data and converted ‘date’ column to date datatype.
	
	Analyzed the start date and end date for each league in each season.
	
	Calculated the duration for which each league lasted in each season. Noted that leagues in 2019 lasted for the most time. ‘Swiss Raiffeisen Super League’ lasted for the 	 greatest number of days
	
	Analyzed the number of matches played in each league in each season. Noted that the most matches were played in ‘United soccer league’ in its 2019 season 			followed by ‘English League championship’ in 2018 season.
	
	Performed linear regression between spi and rank and predicted ranks for the teams. Noted that team ranks are directly related to their spi
	
	Performed gradient boost regression on the data and noted the relation between spi and ranks. 
	
	Using multiple linear regression, derived a relation between xsg, nsxg and adjusted scored and derived the equation for predicting scores.
	
4.	Data Plotting

	Plotted all the predicted data as per linear regression model using a scatter plot
	
	Plotted the actual value using a line graph on the axes to observe the relationship
	
	Plotted all the predicted data using gradient boost regression model using a scatter plot
	
	Plotted the actual value using a line graph on the axes to observe the relationship
	
5.	Conclusion/Inferences
(Feature Engineering) Derived the movies with maximum user ratings and noted that 'Forrest Grump' topped the list with 3518 user ratings followed by 'Shawshank Redemption' with 3488 user ratings
Most users give a rating of 4 stars for movies.
Most movies received a rating between 3 to 4 stars
