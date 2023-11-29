# Final-Group-Project

# Cleaning the Dataset
First order of business is cleaning our dataset. We first attempt to import the pandas library, installing it if necessary.
Then we read the "global_air_pollution.csv" dataset into a pandas DataFrame named df. 
The data preprocessing steps involve dropping the 'Country' and 'City' columns and removing rows with missing values. 
We then define a function to convert categorical AQI values to numeric representations and apply it to specific columns in the DataFrame, transforming AQI categories into numerical values. 
The cleaned DataFrame is then saved to a new CSV file named 'cleaned_dataset.csv', excluding the index column. 
Finally, the script displays the resulting cleaned DataFrame. 
This process ensures that the air pollution dataset is appropriately processed and ready for subsequent analysis or modeling endeavors. 

# Making the Model
The first step in making our model is to import the necessary libraries:
Use Pandas for data manipulation and analysis. Also use Seaborn for some of the visualizations. Then for making the model itself import SciKitlearn train test split, linear regression model and mean squared error as the metric for evaluation. Lastly import matplot for the remaining visualizations. 
The next step is reading the prior cleaned dataset. 
Then assigning our features and target variable, the x-features are the AQI values for each gas(Ozone, NO2, CO and PM2.5) and the target y-value is just the Total AQI. 
Training and testing our model, using 25% of the data for testing. 
Training the linear regression model  on the training set, and generate predictions for the test set. 

# Making the Visualizations
Creating our visualizations using seaborn, depicting scatter plots of the actual vs. predicted total AQI values for each individual pollutant. 
The mean squared error (MSE) is then calculated to assess the model's performance, and a scatter plot is generated to visualize and evaluate the comparison between the actual and predicted total AQI values. 
Finally, the model coefficients are displayed, providing insights into the impact of each feature on the total AQI prediction. 
This script serves as a comprehensive tool for analyzing and visualizing the relationships between different pollutants and the overall air quality index. 
