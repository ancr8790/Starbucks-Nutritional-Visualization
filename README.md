# Starbucks-Nutritional-Visualization
Visualization of Starbucks drinks nutritional information
<br>__[Starbucks Drink Nutritional Information Dataset](ttps://www.kaggle.com/starbucks/starbucks-menu?select=starbucks_drinkMenu_expanded.csv )__

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

In the code cell below, I perform additional tidying of the data.
