# Data-project
Our research question is: What are the prices for adults and children for an activity based on the city and type of activity? 
## Part 1: Webscraping 
To answer our research question, we collected data on activities in Belgium at https://www.365.be/fr. 
This site contains all possible activities in Belgium, whether cultural, natural or recreational. 
On this site we collected the name of all the activities, the city of the activity, the price for an adult, the price for a child and the type of activity (we have 22 different types of activity).
After collecting all this information on the site, we built up a database with a total of 289 data items. 
Finally, we exported our database to an Excel file called "webscraping".

## Part 2: Visualization
We started by making maps. 
The first two maps show where there are activities in Belgium, and the prices at which they are offered. 
The first map is for adults, the second for children. Then we made a map showing all the places where there are activities in Belgium. The last map represents the density of activities according to city. The redder the map, the more activities there are in that city.
Next, we made a scatter plot showing whether there is a relationship between the adult price of an activity and the type of activity.
We've also created a bar chart showing the 20 cities with the most activities in Belgium.
Next, we show the distribution of adult prices according to type of activity, using a box plot to see which types of activity are on average the most expensive or the least expensive, and so on. We do the same for children's prices.
Finally, we made a pie chart to show which types of activities were the most present among all the activities to do in Belgium.
All graph interpretation has been done in the notebook.

## Part 3: Machine learning
In this section, we aim to answer the research question. To do so, we performed a 2 linear regression. 
The first with adult price as the dependent variable and activity type and city as the independent variables. The second with children's price as the dependent variable and the same independent variables. 
These regressions enabled us to see the link between prices, city and type of activity, which in turn enabled us to predict the price of each type of activity in each city. 
We now have a new database with 2728 data items and 4 columns (Type, City, Price prediction for children and Price prediction for adults).
