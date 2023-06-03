# Data-project
Attractions are everywhere. Every person have gone into a museum, an theme park or a zoo. The business of attractions are well widespread. However, the prices for an attraction is different everywhere and depends on a lot of elements. We have then ask ourselves if we can predict the expected price for adult tickets for attractions in a specific city based on the type of attraction and historical pricing data ? This research question explores the possibility of developing a predictive model that utilizes the type of attraction and historical pricing data to forecast the expected prices for adult tickets in a particular city. By investigating this question, researchers can assess the feasibility and accuracy of predicting attraction prices, which can be valuable for various stakeholders such as travel agencies, tourists, and attraction operators. Additionally, this research can contribute to understanding the factors that drive pricing decisions in the tourism industry and enable better resource allocation and decision-making.
We will make an overalll of what have been done in each part of the project. However, there more explanations for each part in the notebook dedicated from each part.
## Part 1 : Webscraping 
To answer our research question, we collected data on activities in the region of Wallonia and Brussels capital at https://www.365.be/fr. 
This site contains all possible activities in region of Wallonia and Brussels capital, whether cultural, natural, or recreational. 
On this site, we collected the name of all the activities, the city of the activity, the price for an adult, the price for a child, and the type of activity. There are a total of 22 different activities listed on the site.
After collecting all this information on the site, we built up a database with a total of 276 data items. 
Finally, we exported our database to an Excel file called "webscraping".

## Part 2 : Visualization
On this part, we are going to make some graphs in order to have some ideas about the situation in Wallonia and Brussels capital.
We have made some maps, bar chart, box plot and a pie chart. All these graphs assess the differences between type of activities or between prices.
All graph interpretation has been done in the notebook.

## Part 3: Machine learning
In this section, we aim to answer the research question. To do so, we performed a 3 linear regression. The three regression have the goal to predict the prices for the adults.
The first regression take as independent variable the city and the type of attractions. The second one add the prices of children to the regression. These two regressions are linear regressions. Then, we use a decision tree regressor with the three independent variables as to know the city, the type of attractions and the prices for children. A decision tree regressor is a specific implementation of decision tree-based models for regression tasks.This algorithm follows the general principles of decision tree construction, recursively splitting the data based on features to minimize the impurity or variance within each subset.
These regressions enabled us to see the link between prices, city, and type of activity, which in turn enabled us to predict the price of each type of activity in each city. 
We now have a new database for the predictions and 4 columns (Type, City, Predicted Adults Prices with model 2, and Predicted Adults Prices with model 3). We have also exported this database with price predictions for adults according to city type of activity and the prices for children, the file is called "predict_df".
We also respond to the questions in the notebook.
