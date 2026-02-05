# Crop Yield Prediction using Machine Learning
1.Problem Understanding:

Agriculture is highly dependent on environmental and operational factors such as rainfall, temperature, pesticide usage, and cultivated area. Accurately predicting crop yield helps farmers and policymakers in planning agricultural activities, managing resources, and ensuring food security.
The objective of this project is to build a machine learning regression model that predicts crop yield (hg/ha) using a real-world agricultural dataset. The dataset contains historical records of crop production along with weather and region-based attributes. By learning patterns from past data, the model can estimate future crop yield values.
This is a supervised learning problem, where:
Input variables (features) include average rainfall, average temperature, pesticide usage, crop type, and geographical area.
Output variable (target) is crop yield measured in hectograms per hectare.
The focus of this project is not only on prediction accuracy but also on:
Proper data preprocessing
Model selection
Evaluation using standard metrics
Explaining how the model arrives at predictions

2.Model Pipeline Description:
   
The complete machine learning pipeline followed in this project is explained below:
Step 1: Data Collection
A publicly available crop yield dataset was used.
The dataset was loaded using Pandas for analysis and preprocessing.
Step 2: Data Preprocessing
Removed unnecessary columns (such as index columns).
Checked and handled missing values.
Encoded categorical variables like Area and Crop Item using Label Encoding.
Created new features (feature engineering) to capture combined effects of rainfall, temperature, and pesticide usage.
Step 3: Feature Selection
Selected relevant numerical and encoded categorical features.
Defined:
X → input features
y → target variable (crop yield)
Step 4: Train-Test Split
Dataset split into:
80% training data
20% testing data
Ensured reproducibility using a fixed random state.
Step 5: Feature Scaling
Applied StandardScaler to normalize numerical features.
Scaling helps models converge faster and improves stability.
Step 6: Model Training
Trained two regression models:
Linear Regression (baseline model)
Random Forest Regressor (advanced ensemble model)
Models were trained using the training dataset.
Step 7: Model Evaluation
Predictions generated on test data.
Performance evaluated using regression metrics.
Step 8: Inference & Interpretation
Compared predicted and actual yield values.
Used feature importance from Random Forest to explain model behavior.

3.Results & Metrics:

The performance of both models was evaluated using standard regression metrics:
Evaluation Metrics Used
Mean Absolute Error (MAE) – Average prediction error
Root Mean Squared Error (RMSE) – Penalizes larger errors
R² Score – Measures how well the model explains variance in crop yield
Observed Results
Linear Regression provided a baseline performance.
Random Forest Regressor performed better due to its ability to capture non-linear relationships.
Features such as rainfall, temperature, and cultivated area showed high influence on crop yield.
The evaluation confirms that the model successfully learns patterns from historical data and provides reasonable yield predictions.

4.Code (GitHub / Colab):

The complete implementation of this project is available in a Google Collab, which includes:
Data preprocessing
Feature engineering
Model training
Evaluation
Visualization and inference
Files Included
yield_df.csv – Dataset
AI&ML.ipynb – Complete code



