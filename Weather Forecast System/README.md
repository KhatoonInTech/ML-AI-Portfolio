# ***Report: Weather Classification Model***
---

  >> Introduction

        The dataset used in this project consists of 13,200 samples with 15 features, including temperature, humidity, wind speed, and other weather-related attributes.
        The objective is to develop a classification model that can accurately predict the weather type (Cloudy, Rainy, Snowy, or Sunny) based on these features.

  >> Data Cleaning and Preparation

        The dataset was split into training and testing sets using an 80-20 split, resulting in 10,560 samples for training and 2,640 samples for testing.
        The data was then normalized using Min-Max Scaling to ensure that all features were on the same scale.

   >> Data Analysis and Visualization

        Exploratory Data Analysis (EDA) was performed to identify key patterns, correlations, and insights in the data. The following insights were obtained:

              The dataset has 15 features, with temperature and humidity being the most correlated features (correlation coefficient: 0.85).
              The box plot of numerical features showed that the data has some outliers, but they were not extreme enough to warrant removal.
              The correlation heatmap revealed that there are some strong correlations between certain features, such as temperature and humidity, and wind speed and atmospheric pressure.
    
  >> Model Building

        Three classification models were built and trained on the dataset:
            1. Logistic Regression
            2. Decision Tree
            3. Random Forest
            
        The training process involved tuning hyperparameters to optimize model performance.

  >> Model Evaluation

        The performance of each model was evaluated using accuracy, precision, recall, and F1-score. The results are as follows:

              Logistic Regression:
                  Accuracy = 0.850758
                  Precision = 0.850794
                  Recall = 0.850758
                  F1-score = 0.850226

              Decision Tree:
                  Accuracy = 0.908333
                  Precision = 0.908449
                  Recall = 0.908333
                  F1-score = 0.908358

              Random Forest:
                  Accuracy = 0.921970
                  Precision = 0.922034
                  Recall = 0.921970
                  F1-score = 0.921994

  >> Best Performing Model

          The Random Forest model outperformed the other two models,
          achieving an accuracy of 92.20%.
          The classification report for the Random Forest model is as follows:

              Cloudy:
                Precision = 0.905109, Recall = 0.911764, F1-score = 0.908424
              Rainy:
                Precision = 0.917159, Recall = 0.914454, F1-score = 0.915805
              Snowy:
                Precision = 0.941984, Recall = 0.934848, F1-score = 0.938403
              Sunny:
                Precision = 0.924679, Recall = 0.927652, F1-score = 0.926163
  >> Conclusion

         > The Random Forest model was found to be the best performing model,
         > achieving an accuracy of 92.20%.
         > The model effectively learned the patterns in the data and made accurate predictions about the weather type.
         > The results suggest that the model can be used for weather classification tasks.
         
         Future work
            could involve collecting more data to improve the model's performance and exploring other machine learning algorithms to compare their performance with the Random Forest model.

