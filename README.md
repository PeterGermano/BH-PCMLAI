# What drives the price of a used car?

##Business Understanding

Rudy Russo has a problem. We've seen how bad business is. Thanks to Fuchs, his name is mud.

Something that may help Rudy is to accurately price used cars as appropriately priced cars tend to sell faster.

By leveraging existing data, we can build a supervised learning model using the sale price for predictions.

  ###The analysis will highlight factors influincing the price
  ###The model will then identify the correlations that impact pricing
  ###A validated model can then be used to provide informed pricing on prospective vehicles.
  
##Data Understanding

The initial dataset contains 426,880 entries with 17 columns
 0   id             
 1   region        
 2   price          
 3   year          
 4   manufacturer   
 5   model         
 6   condition     
 7   cylinders     
 8   fuel           
 9   odometer     
 10  title_status  
 11  transmission  
 12  VIN            
 13  drive          
 14  size          
 15  type         
 16  paint_color    
 17  state         
 
The dataset was reviewed to identify the columns relevent to the modeling exercise and resulted in the removal of ID and Vin. Both are unique identifiers that don't inform the price. 
Next, the data was cleaned to contain only lowercase letters and remove spaces.
Null values were imputed using central tendency measures for numeric features and Bayesean regression for categorical features.
As the price is the central feature for implementing the model, the distribution of prices in the dataset were specifically explores.  It was determined the a log transform provides a normal distribution. Prices were also limited to the interquartile range (IQR) to represent the spread of the middle half of the prices and remove 0 and outlier values outside the range.
The final cleaned and prepped dataset contained 82440 entries that were used in the model.

 
##Evaluation
The dataset can support building a model.

The current dataset is limited by inconsistancies in the variables.

Correlations have been identified to predict price but the data treatment and fitting require further investigation.

An approriate data cleaning process that identifies relevant factors and the fit to a strong model can be identified. Linear regression fits with approx. 62% accuracy. The random forest model is an improvemnt over the linear regression model with a fit of 88%.

Alternate methods of analysis using k-nearest neighbors, cluster analysis, primary component analysis or polynomial fitting can be used and may provide stonger models.

##Deployment
The factors that are involved in pricing (car age, milage, and size) are intuitive pieces of the price. The subltety of their influence, however, is not easily discerned. As demonstrated by the models, a correlation and fit can be derived from the relationship of the price these factors. The best fitting models have a fit of 88%. Additional investigation into why the correlations exist and how they can be applied to beat the "human gut feeling" is warranted.
