# Bike-Sharing-Demand-Prediction

Bike sharing demand prediction

Problem Description:
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

Data Description:
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.


Attribute Information -

Date : year-month-day

Rented Bike count - Count of bikes rented at each hour

Hour - Hour of the day

Temperature-Temperature in Celsius

Humidity - %

Windspeed - m/s

Visibility - 10m

Dew point temperature - Celsius

Solar radiation - MJ/m2

Rainfall - mm

Snowfall - cm

Seasons - Winter, Spring, Summer, Autumn

Holiday - Holiday/No holiday

Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

#Steps for Model Building

1]Reading and Understanding Data

2]Visualising the Data

3]Data Preparation

4]Splitting the Data into Training and Testing Sets

5]Feature Scaling on the train data

6]Building the Model

7]Analysis of the train data

8]Best features for prediction

9]Model Evaluation

FINAL OBSERVATION

1.People generally use more number of rented bikes during from 7 AM - 9 AM and 5 PM- 8 PM r as it is office start and end time.

2.In summer more number of bikes are rented whereas, winter has the lowest count.

3.Least numbers of bike are rented on sunday as its holiday.

4.More bikes are rented if the humidity is low and wind-speed is high.

5.Rainfall and snowfall impact the number of bikes rented tremendously with very high downfall.

6.we can say that temperature has a highest weightage then Hour and humidity.

7.Linear regression is not suitable for our problem as it makes many assumptions and our dataset is prone to it. Thus, linear regression gives us the lowest r2-score and highest rmse.

8.Random forest regressor performs really good when compared to linear regression with high model performance and low rmse. But it's performance is low when compared to gradient boosting regressor. However, time taken for hyperparameter tuning and training the model is much low for random forest regressor than gradient boosting regressor. Thus, there's a tradeoff of accuracy and time in between random forest and gradient boosting regressor. It's up to us and business domain to which
algorithm to use.

9.Out of all above models Gradient Boosting Regressor gives the highest R2 score of 97.5% for Train Set and 92.0% for Test set and no overfitting is seen.
