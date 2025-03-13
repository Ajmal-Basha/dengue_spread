Dengue Disease Prediction Project
Overview
This project aims to predict the spread of dengue disease in Chennai, using a variety of techniques such as geospatial data visualization, machine learning classification, time-series forecasting, and predictive modeling. The model predicts future trends in dengue outbreaks based on historical data, risk levels, and external factors like weather patterns and sanitation data.

Project Structure
The project contains the following components:

Data: Contains datasets on dengue cases in Chennai, including risk levels, case counts, and location-based data.
Model: Trained machine learning models to classify and predict dengue risk levels.
App: A Flask-based web application for real-time predictions and visualization.
Scripts: Python scripts for data processing, model training, and prediction.
Key Features
Risk Level Classification: The project classifies areas in Chennai based on the number of dengue cases (low, medium, high, very high).
Prediction of Disease Spread: Uses XGBoost and other models to predict future dengue trends.
Geospatial Visualization: Interactive maps to visualize the affected areas and predict future hotspots for dengue.
Real-time Predictions: A Flask app to input new data and predict the dengue risk in real-time.
Dependencies
The following Python libraries are required to run the project:

pandas
numpy
scikit-learn
xgboost
flask
matplotlib
seaborn
geopandas
folium
plotly
scikit-learn
Install these dependencies via pip:

nginx
Copy
Edit
pip install -r requirements.txt
Datasets
updated_dengue_data_with_risk_level.csv: Historical dengue case data with added risk levels.
future_dengue_predictions.csv: Dataset used to predict future dengue cases based on historical trends.
trained_dengue_model.pkl: The trained machine learning model used for predictions.
How to Run
Clone the repository:

bash
Copy
Edit
git clone <repository_url>
cd <project_directory>
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the Flask app:

bash
Copy
Edit
python app.py
Access the web app at http://127.0.0.1:5000/.

Hyperparameter Tuning
The model has been optimized using hyperparameter tuning techniques to improve its performance. The following parameters were tuned:

Learning Rate: Adjusted to control the contribution of each tree in the ensemble.
Max Depth: Determined the maximum depth of each decision tree.
Number of Estimators: Optimized the number of trees in the model.
Future Enhancements
Advanced Models: Exploring the use of LSTM or GRU for better time-series forecasting.
Feature Engineering: Incorporating additional features such as weather patterns, mosquito indices, and sanitation data.
Spatial Clustering: Implementing zone-wise predictions based on geographical clustering.
License
This project is licensed under the MIT License - see the LICENSE file for details.
