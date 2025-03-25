# 🎬 Movie Rating Prediction

## 📌 Objective
This project aims to develop a machine learning model that predicts movie ratings based on various attributes such as duration, genre, votes, and key personnel (director, actors, etc.). The goal is to provide insights into factors influencing movie ratings and create a reliable predictive tool.

## 📂 Dataset
The dataset used is **IMDb Movies India.csv**, which contains detailed information about Indian movies, including:
- **Duration**: Length of the movie in minutes.
- **Votes**: Number of votes received on IMDb.
- **Genre**: Categorized genre of the movie.
- **Director**: Name of the director.
- **Actor 1, Actor 2, Actor 3**: Lead actors in the movie.
- **Rating**: IMDb rating of the movie (Target variable).

## 🔧 Data Preprocessing
To ensure high-quality input data, the following preprocessing steps are performed:
✅ Convert categorical variables into numerical representations.
✅ Handle missing values:
   - Numerical columns are filled with their **median** values.
   - Categorical columns are replaced with **'Unknown'** where missing.
✅ Encode categorical features using **Label Encoding**.
✅ Normalize data where necessary to improve model performance.

## 🤖 Model Implementation
A **Random Forest Regressor** is used as the predictive model due to its high accuracy and robustness with structured data. The dataset is split into **training (80%)** and **testing (20%)** sets.

### 🔍 Why Random Forest?
- Handles missing data effectively.
- Reduces overfitting compared to decision trees.
- Works well with categorical and numerical features.

## 🚀 How to Run the Project
### 1️⃣ Install Dependencies
Ensure you have the required libraries installed by running:
```sh
pip install pandas numpy scikit-learn
```

### 2️⃣ Run the Python Script
Execute the following command:
```sh
python movie_rating_prediction.py
```

## 📊 Model Evaluation
The model performance is assessed using the following metrics:
- **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted ratings.
- **R-squared Score (R²)**: Determines how well the model explains variance in ratings.

## 🎯 Expected Outcome
This project aims to produce a machine learning model that accurately predicts movie ratings based on input attributes, helping filmmakers and analysts understand the key factors influencing a movie's success.

## 🚀 Future Enhancements
🔹 Incorporate additional features such as director success rate, production budget, and box office earnings.
🔹 Experiment with other regression models like XGBoost and Neural Networks.
🔹 Optimize hyperparameters using Grid Search or Bayesian Optimization.

## 📢 Conclusion
This project effectively demonstrates how machine learning can be leveraged to predict IMDb ratings, providing valuable insights into the movie industry. The structured approach ensures readability, efficiency, and scalability.

Mean Squared Error: 0.7855670279613511
R-squared Score: 0.192144021267386



