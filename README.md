# Stroke-Prediction-Modeling

## Predicting the risk of having a stroke based on a multitude of variables

**Alexander Re** 

### Business problem:

How do characteristics such as age, blood-glucose levels, what you do for work, and where you live impact your risk of having a stroke?


### Data Source: 
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset


## To prepare this data, the data was cleaned, and the following processes were performed:


### Explanatory Data Analysis
#### - A countplot was used to visualize the number of people in the dataset had a stroke compared to the number who did not have a stroke.
#### - Histograms, boxplots, or countplots were used on all categorical data.
![](Screen%20Shot%202023-03-02%20at%209.20.43%20PM.png)
> The countplot shows that the majority of people in the dataset did not have a stroke. This indicates how imbalanced the data is. 


### Exploratory Data Analysis
#### - This line graph shows the relationship between age and the amount of strokes in patients.
![](Screen%20Shot%202023-03-02%20at%209.21.02%20PM.png)
> This graph shows that as age increases, there is also an increase in the amount of patients who had strokes.  


#### - This bar graph shows the relationship between patients who have hypertension and those who have had strokes.
![](Screen%20Shot%202023-03-02%20at%209.42.53%20PM.png)
> This graph shows that patients who have hypertension are much more likely to have a stroke than those who do not have hypertension. 


## Model

The model used was a KNN Model. 

### Important metrics
#### Train
- Precision: 0.50
- Recall: 1.00
- Accuracy: 0.96
#### Test
- Precision: 0.00
- Recall: 1.00
- Accuracy: 0.96

>This model did not perform well on the test data set. The accuracy score is decieving. Even though in the test set, the model was correct 100% of the time when predicting true negatives, the test set did not predict any true positives correctly. This is an issue, because it is dangerous to have a model that incorrectly predicts that a person will not have a stroke, when they are clearly at high risk of having one. 


## Recommendations:

Based on the exploratory data, I reccommend that screenings and tests for stroke likelihood be increased as a patient's age increases. There is a clear correlation between a patient's age and their risk of having a stroke. I would also recommend that patients who have hypertension be closely monitered, as the bar graph above indicates that their risk of having a stroke is much higher than those who do not have hypertension. 

## Limitations & Next Steps

The largest limitation with the model and the dataset was that there was significantly more data on those who did not have strokes than those who do. This imbalance caused the model to be inaccurate when predicting true positives. In the future, I will use techniques to balance the dataset so that the model can make better predictions. 
