# Final-Group-Project

# Cleaning the Dataset
First order of business is cleaning our dataset. We first attempt to import the pandas library, installing it if necessary.
Subsequently, we read the "global_air_pollution.csv" dataset into a pandas DataFrame named df. 
The data preprocessing steps involve dropping the 'Country' and 'City' columns and removing rows with missing values. 
We then define a function to convert categorical AQI values to numeric representations and apply it to specific columns in the DataFrame, transforming AQI categories into numerical values. 
The cleaned DataFrame is then saved to a new CSV file named 'cleaned_dataset.csv', excluding the index column. 
Finally, the script displays the resulting cleaned DataFrame. 
This process ensures that the air pollution dataset is appropriately processed and ready for subsequent analysis or modeling endeavors. 

# Making the Model
The first step in making our model was to import the necessary libraries:
Used Pandas for data manipulation and analysis. We had to use Seaborn for some of the visualizations. Then for making the model we used SciKitlearn train test split, linear regression model and mean squared error as the metric used for evaluation. Lastly we imported matplot for the remaining visualizations. 
The next step was to read the prior cleaned dataset. 
Then assigned our features and target variable, the x-features were the AQI values for each gas(Ozone, NO2, CO and PM2.5) and the target y-value was just the Total AQI. 
Trained and tested our model, using 25% of the data for testing. 
Trained the linear regression model  on the training set, and predictions were generated for the test set. 

# Making the Visualizations
Our visualizations were created using seaborn, depicting scatter plots of the actual vs. predicted total AQI values for each individual pollutant. 
The mean squared error (MSE) was then calculated to assess the model's performance, and a scatter plot is generated to visualize and evaluate the comparison between the actual and predicted total AQI values. 
Finally, the model coefficients were displayed, providing insights into the impact of each feature on the total AQI prediction. 
This script serves as a comprehensive tool for analyzing and visualizing the relationships between different pollutants and the overall air quality index. 
