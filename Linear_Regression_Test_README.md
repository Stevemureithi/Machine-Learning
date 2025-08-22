# Linear Regression Test
##### About the data
The dataset explores several attributes of different car brands, including their names, selling price, year of manufacture, mileage, engine ratings, maximum power, number of seats, ages, transmission types, and distances driven. Owners and seller type details are also provided.

##### Data Cleaning and Preprocessing Section:

This section included bits on loading CSV files in pandas, checking the data types, looking for missing values, using the right column formats, and checking for inconsistencies in the data. 
The key insights from this section include 
⦁	The datatypes were float64, int64 and object
⦁	The mileage, engine, max power, and seats columns had missing values.
⦁	There were duplicated rows (these were removed).
⦁	Numerical columns were stored correctly.

##### Exploratory Data Analysis (EDA) Section:

This section included basic manipulations and calculations using the data. There are several data visualizations in the section as well.

Key insights:
⦁	The average car price is slightly over half a million
⦁	Most cars run on diesel.
⦁	The selling price data is not normally distributed.
⦁	There is an inverse relationship between the selling price and the age of cars, with newer cars costing more than older ones.
⦁	Different selling prices by fuel type, with diesel-run cars costing more.
⦁	Manual cars are the majority in the dataset.
⦁	There is a weak negative correlation between mileage and selling price.
⦁	No high/strong correlation between the numerical columns.
⦁	Automatic cars cost more than manual cars.
⦁	Newer cars cost more.
⦁	Car prices declined  relatively from 1985 and before to 2000 before surging up to 2019.

##### Machine Learning Section:

Tasks completed in this section included using linear regression, Lasso & Ridge regression models to predict the selling price of cars.
 
Key Insights:
⦁	The residuals scatter plot shows a linear association of the residuals, meaning the model is contravening  
⦁	Variance score of 1 = perfect prediction, thus the linear regression model can be relied upon.
⦁	R-squared is 1; therefore, the model provides a perfect prediction and is reliable. (Caveat is the risk of overfitting by the model)
⦁	The Lasso model performs better due to the size of errors. The errors are more plausible given the scale of the target column in the dataset. The selling price range includes amounts in tens of thousands, hundreds of thousands and millions. Lower errors in Linear regression and Ridge models show potential overfitting of the data-The data is almost too perfect for the models to explain 100% of the variance (R2=1), suggesting overfitting or issues in evaluation of the data. While the errors in the Lasso model are also small compared to the selling price figures, they are more plausible than the other two models.
