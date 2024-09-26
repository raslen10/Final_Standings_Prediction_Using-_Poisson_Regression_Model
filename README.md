# Final_Standings_Prediction_Using-_Poisson_Regression_Model

Project Overview
This project aims to predict the final standings of the Premier League using match data collected from the 2020 to 2024 seasons. By leveraging a Poisson regression model, we estimate the number of goals scored by each team in individual matches, which then helps us simulate and predict the overall league standings at the end of the season.

Data Collection
The match data was collected using the requests library from various online sources, ensuring comprehensive coverage of all matches played from the 2020 to 2024 Premier League seasons. The dataset includes information such as:

Match date
Home team
Away team
Goals scored by each team
Methodology
Data Preprocessing:

Cleaning and structuring the raw data to ensure consistency.
Handling missing values and potential discrepancies in team names and match details.
Feature Engineering:

Creating features such as home advantage, team strength, and opponent strength.
Encoding categorical variables (e.g., team names) for use in the model.
Modeling:

Utilizing a Poisson regression model to predict the number of goals scored by each team in a match.
The Poisson model is chosen because the distribution of goals scored in a match typically follows a Poisson distribution.
The model formula used is:

log
⁡
(
𝜆
)
=
𝛽
0
+
𝛽
1
⋅
home
+
𝛽
2
⋅
team
+
𝛽
3
⋅
opponent
log(λ)=β 
0
​
 +β 
1
​
 ⋅home+β 
2
​
 ⋅team+β 
3
​
 ⋅opponent
where 
𝜆
λ is the expected number of goals scored.

Simulation:

Simulating the results of the entire season using the predicted number of goals for each match.
Aggregating the match results to calculate the total points for each team and determine the final standings.
Results
The model provides predicted final standings for the Premier League based on the simulated match outcomes. These predictions can be compared to actual historical standings to assess the model's accuracy and make necessary adjustments for future predictions.


Contributing
We welcome contributions from the community. If you find a bug or have a feature request, please open an issue. Feel free to fork the repository and submit pull requests for any enhancements.
