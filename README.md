Hello!
Have you ever wondered how many medals your country would get in the Olympics? And thought that maybe there was a way to find it for real. Well, Machine Learning does that for you, by taking the previous data and studying it very carefully we can estimate that with good precision rates.
So, let's break down what really happens in this...
There is a popular machine-learning methodology called Linear Regression, which basically relates two variables, based on the previous data, if we can somehow put the two variables Country and Previous medals into the model alongside the output medals in that particular  year, we can train a model that can predict the values of the country medals.
And now is the time to figure out how exactly...
There are seven steps for that, It may sound complex on a bigger picture but on an organized scale, it is easy to do.

1. FORM A HYPOTHESIS
   Basically, the hypothesis is the specific explanation for a problem statement. And the hypothesis is defined by past data.
And our HYPOTHESIS here is that we can build a model that can predict the medals for a country.

2. FINDING THE DATA 
   Mining the data and fetching the data from multiple sources show different aspects and factors of the data, in this model we are training the model not to get the output but to predict the output for the future, in other words, Linear regression is a supervised machine learning model, which basically takes input and output as well of the current data and can predict the future prices. So we are providing the medals won by the country in past and present years and training the model to predict the future.

3. RESHAPING DATA
   Reshaping data means organizing the aspects in the columns in a specific way where pulling the data is simple preventing any confusion.

4. CLEANING THE DATA
   Data cleaning is such an important step in building models which directly impacts the precision of the models. In the real world, the data always has duplicates in it for instance we are looking at the data of teams performing Olympics It is not like every team participating gets a medal, which means there would be many countries without winning a single medal in the Olympics and such 0 values affect the precision of the model so dropping the duplicates thereby cleansing the data is a very essential step in order to get high precision model.

5. ERROR METRIC
   Error metric here is using mean absolute error in here, as at last all the data is averages and statistical values hence it always has errors involved in it. Here we predict the potential number of medals that will win, the difference between the actual medals and predictions is the error, for example, if the real data we have shows the country has won 4 medals in a year and the predictions say it is 7 the difference between these variables are 3 and that is the error. We add all the errors for each row and divide the total by the number of rows giving the mean absolute error and adjusting the predictions with these errors predicts the values more accurately.

6. SPLITTING THE DATA
   The question gives all the answers. Here we split the data into two. WHY?. The data is split into two parts A and B, 80% of the data goes to A and 20% goes to B. In order to check the precision, when we train the model with A and test it with B. As we already have the values or answers (no.of medals) we can check the predictions and measure their precision thereby adjusting the error metric.

7. TRAIN THE MODEL
   Y= aX + b
   Simple equation with a great potential here X and Y are the variables that we are trying to predict.
   The intersections of these two values are plotted on a graph and a line is passed with an average slope with relevant to that data point. Thereby having a reference for future predictions.
