# Data Mining Group Project :)
Carvana is an online used car dealership in the United States that buys and sells used cars through your devices or their famous car vending machines. For this project, our team at Hawkeye Consulting collaborated with Carvana to help set the prices for their used car inventory.  

### Background
At Hawkeye Consulting we aim to give solutions to our clients through data visualization and driven recommendations. Therefore, we partnered with Carvana, a used car dealership. Carvana is currently the fastest growing online used car dealership in the US and is mainly known for their car vending machines. Additionally, according to CNBC, American consumers have been paying $10,000 more on average for used cars. The Covid-19 pandemic and the current microchip shortage help explain this. The microchip shortage is causing a new car shortage due to the fact that microchips are an essential part of manufacturing. When consumers physically cannot buy new cars, they are forced to choose from the used car market, one that is known to overprice their products. Mileage is the first thing that comes to mind when thinking about used car prices, however we wanted to determine what other factors contribute to the price of a used car. 

### Data
The raw dataset is from Kaggle.com, is named the Car Price Prediction Challenge, contains 19237 instances, and 18 features. The original dataset includes features such as manufacturer, model, production year, mileage, color, etc. After the data was cleaned, it contained 2000 instances with 10 categorical features and 6 numeric features. Price is our target variable. 

#### Data Pre-Processing
Step 1: Removed nonsensical data. 

- Nonsensical data : Removed unrealistic price data i.e., cars made later than 2010 with a listed price under $1000. This assumes no cars in the dataset needed significant repair. 

Step 2: Corrected data format. 

- Format correction: The ‘doors’ column was formatted as a date. Changed format to integer. 

Step 3: Decreased the number of observations to 2000.  

Step 4: Changed target variable to categorical. 

- Target variable: Changed all values in the ‘price’ column to cheap or expensive. Values greater than or equal to the median price, $15,000, were changed to expensive. Values less than the median price, $15,000, were changed to cheap. 

### Data Mining Solution
Through various models we were able to find various attributes in a car that affected whether or not the price would go up or down. Airbags, right-hand drive, and levy were the top three most important variables affecting price in our model. Carvana does not currently have all of these things listed in their description of their cars and could potentially be losing or missing sales because of it. 

### Models
We tested three separate models in order to find the best predictor for whether or not a car would be placed in the expensive or cheap category. 
- Decision Tree 

- Random Forest 

- SVM 

### Conclusion
To conclude, we discussed how a high percentage of cars are being sold at a premium. From there, we set our business goal to see what additional factors can impact a car's price. Using a Random Forest, Decision-Tree and SVM model we were able to interpret our dataset and find factors with importance to form our overall recommendations and limitations to our set.  

#### Recommendations
After creating a Random Forest, Decision-Tree, and SVM model based on our findings, we recommend that Carvana focus their purchasing and marketing strategy around safety, interior quality, fuel size, and size class. Based on our dataset, we found that car safety has a higher mean decrease accuracy when performing a random forest model. This helped form an overall recommendation based around safety to adequately show the variable importance represented in our random forest model. The same can be said for fuel size because of the importance it has when customers purchase a car. Also, interior quality and size class are recommended when focusing on purchasing and marketing strategies because of the appeal it can have on customers. This can lead to higher increases in revenue and marketing appeal. 
