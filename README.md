# House-price-Prediction
California House Price Prediction

This repository contains a Jupyter Notebook (House_price_prediction.ipynb) that implements a machine learning workflow to predict house prices using the California Housing dataset from scikit-learn. The project is designed for data scientists and developers to explore data preprocessing, visualization, model training, and deployment using Python. It provides a reproducible example of building a predictive model with a focus on clarity and best practices.

Project Overview

The notebook uses the California Housing dataset, which includes features like median income, house age, and average rooms to predict house prices. The workflow begins by loading the dataset into a pandas DataFrame using fetch_california_housing() from sklearn.datasets. Initial data exploration is performed with df.head() to verify the data structure, followed by visualization using matplotlib and seaborn to uncover relationships between features and the target variable (house prices).

Data Preparation and Modeling

The dataset is cleaned and prepared for modeling, addressing any missing values or inconsistencies. The data is then split into training and testing sets to evaluate model performance on unseen data. A Random Forest model is trained using scikit-learn, and its performance is assessed using metrics such as Mean Squared Error and R² score. This ensures the model’s predictions are accurate and generalizable.

Model Persistence

The trained Random Forest model is saved as recalculated_tuned_house_price_model.pkl using joblib. This allows the model to be reused or deployed without retraining, making it suitable for production environments or further experimentation. The notebook ensures all steps are well-documented for reproducibility.

Installation and Usage

To run this project, ensure you have Python 3.8+ installed. Clone the repository and install the required dependencies listed in requirements.txt:

git clone <repository-url>
cd <repository-directory>
pip install -r requirements.txt

Then, launch Jupyter Notebook and open House_price_prediction.ipynb:

jupyter notebook

Execute the cells sequentially to load the dataset, preprocess the data, train the model, and save the results. The California Housing dataset is fetched directly from scikit-learn, so no external data files are required.

Requirements

numpy
pandas
matplotlib
seaborn
scikit-learn
joblib

Contributing

Contributions are welcome! Please open an issue to report bugs or suggest improvements, or submit a pull request with your changes. Ensure your code follows the project’s structure and includes appropriate documentation. For major changes, please discuss them in an issue first.
