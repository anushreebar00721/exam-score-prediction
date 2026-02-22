# exam-score-prediction
***1. Problem Statement***

The goal of this project is to build a machine learning model that predicts a student's Exam Score based on key academic and lifestyle factors such as Hours Studied, Sleep Hours, and Attendance. This project aims to understand how these features influence performance and use Linear Regression to create a simple, accurate prediction system.

***2. Dataset Description***

This dataset contains information about 15 students and their academic habits.
The goal is to analyze how different factors influence Exam Score.

Features Used
| Feature                            | Description                                                     |
| ---------------------------------- | --------------------------------------------------------------- |
| **Hours_Studied**                  | Daily study hours                                               |
| **Sleep_Hours**                    | Average number of hours the student sleeps                      |
| **Attendance**                     | Attendance percentage in class                                  |
| **Exam_Score**                     | Final exam score (target variable)                              |
| **Practice_Tests** *(added later)* | Number of practice tests attempted (new feature for experiment) |

This is a manually generated dataset created for ML practice and model experimentation.


***3. Model Used***

This project uses a Linear Regression model to predict student exam scores based on features such as hours studied, sleep duration, attendance percentage, and an additional feature for practice tests taken. The model was trained using an 80-20 train-test split and evaluated using MAE and R² score.

***4. Results***

The model achieved an MAE of about 3.30 and an R² score of 0.93 using all three main features.
Removing the Sleep_Hours feature slightly reduced the performance.
Adding the Practice_Tests feature improved the accuracy of the model.
Training on the full dataset without splitting showed a much lower MAE and a very high R², which indicates overfitting.


***5. Conclusion***

The experiment shows that Hours_Studied and Attendance are the most influential features for predicting exam performance, while adding additional meaningful features like Practice_Tests can further improve accuracy. The large difference between split-model performance and full-data performance highlights the importance of using proper train-test splits to avoid overfitting. Overall, the linear regression model performs reliably and provides meaningful insights into the factors affecting exam scores.
