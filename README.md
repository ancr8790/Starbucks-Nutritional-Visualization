# Starbucks-Nutritional-Visualization
Visualization of Starbucks Drinks Nutrition 

Starbucks Drink Nutritional Information Dataset: https://www.kaggle.com/starbucks/starbucks-menu?select=starbucks_drinkMenu_expanded.csv

The dataset I chose to work with describes the drinks offered at Starbucks, a popular café, along with their nutritional information. This data in csv format was found on Kaggle. It features the drink categories and their respective sizing. Additionally, it features standard nutritional information found on most food and beverages in America: 
<br>- Calories 
<br>- Total Fat
<br>- Trans Fat
<br>- Saturated Fat
<br>- Sodium
<br>- Total Carbohydrates
<br>- Cholesterol
<br>- Dietary Fiber
<br>- Sugars
<br>- Protein
<br>- Vitamins A & C
<br>- Calcium
<br>- Iron
<br>- Caffeine

My goals for working with this data is determine the healthier & unhealthier drinks offered at Starbucks, while considering a holistic nutritional approach. On Kaggle, some exiting histograms existed for illustrating the distribution of the drinks based on each nutritional category. It gives a good initial idea of how the drinks are distributed across each nutritional category, but it appears that a deep diver is required to identify specific characteristics and connections between nutritional categories, drink type categories, or drink preparation styles. Some difficulties were encountered with the way the data set classified “Beverage_prep.” The data does not have iterative-friendly method of classification. It included, in certain cases, both the size and the milk/milk-alternative added. Additionally, the data set listed the drinks in a way that only mentioned the size in the preparation that included Nonfat milk. The milk-alternative preparations under the previously listed Nonfat drink were assumed to be the same size, which works for a static numeric table but not so well for plotting.

The tasks I want to complete with the data includes presenting the most relevant nutritional information of the overall Starbucks drink menu and presenting this same information for different drink categories. The purpose of pursuing the presenting this data to communicate to people of drinks to indulge in and drinks to avoid. Identification by drink category is being pursued to give people the option to narrow down their choices without feeling restricted. The tasks will be conducted largely by organizing data. These tasks seek to identify patterns across drink category types, drink preparations with nutritional information. Operation of these tasks occurs across a relative reference frame as the data point’s nutritional information will be compared against each other to inform the user of the best and worst drink choices in the dataset. The tasks will be performed by the data analyst, after the dataset is cleaned up and made more uniform. 

Specific code for data cleaning and visualization can be found in the jupyter notebook attached. 

The first attempt at visualization involved getting some simple counts of drink numbers in Beverage_category and Beverage_prep
![drinkCountchart | drinkPrepCountchart](https://user-images.githubusercontent.com/95835246/178845795-83419ea8-e8c4-43d2-afae-32bcc878a208.png)

In trying to figure out how to filter out the data set most efficiently, I found two different ways to filter. The first was was to iterate through the entire data set using 'for' and 'if' loops. This proved to be inefficient with loss of certain information. The second way I tried to filter was by making separate data frames where the column categories was limited to one value. 

I then proceeded to write up a function that would load nutritional charts displaying Calories, Total Fat, Sugars, and Caffeine content of drinks in specific categories. 
![makeNUTchart(CED)](https://user-images.githubusercontent.com/95835246/178845976-a17bb409-85c9-4ff3-8639-645268532dd9.png)

Unfortunately, I realized that this would require user input to be fed into the code realm, which again did not seem to be the most efficient method to present data. After additional research, I was able to implement filtering in the form of Altair's selction capabilities. I utilized a multi_selection by color in the legend to filter out the Beverage preparations and a single_selection using a dropdown menu to filter out the Beverage categories.
![totalPlot encode](https://user-images.githubusercontent.com/95835246/178845988-2c6550b0-8533-4749-901c-e3061c528b93.png)
