This repository contains my contribution to a collaborative MS Applied Data Science capstone project. I worked on data ingestion, feature engineering, and regression model development.

# Capstone Project: Predicting YouTube Video Popularity

This project aims to predict the popularity of YouTube videos using publicly available metadata. By analyzing keywords, publication time, and channel statistics, we use machine learning models to estimate expected video views.

## Project Structure

```
capstone_project/
│
├── Main_Notebook.ipynb # Project overview with links to each section
│
├── Code_Library/
│ ├── Data_Preparation.ipynb # Collects YouTube video data using the API
│ ├── Data_Exploration.ipynb # Cleans and explores the dataset
│ └── Modeling.ipynb # Trains regression models and evaluates performance
│
├── Data_Folder/
│ ├── youtube_videos.csv # Full scraped dataset
│ ├── youtube_videos_1000.csv # Sample dataset (1,000 rows)
│ └── preprocessed_youtube_data.csv # Cleaned version used for modeling
│
├── Other_Material/
│ ├── youtube_api_setup.ipynb # Initial API key setup and test
│ └── catboost_info/ # CatBoost output and logs
```

## Models Used

- Linear Regression
- Support Vector Regression (SVR)
- XGBoost Regressor
- CatBoost Regressor

Each model was evaluated using:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score
- MAPE (Mean Absolute Percentage Error)

## Tools & Libraries

- Python (pandas, numpy, matplotlib, scikit-learn)
- YouTube Data API v3
- XGBoost, CatBoost, SVR
- Jupyter Notebooks

## Notes

- API key is **not included** in this repository. To run the data collection notebook, create an `api.py` file in `Other_Material/` with your own YouTube API key:

```python
API_KEY = "your_api_key_here"
```

## How to Run

1. Clone this repo

2. Set up your virtual environment and install dependencies:
pip install -r requirements.txt

3. Add your own api.py file with an API key

4. Run Main_Notebook.ipynb to explore each step of the pipeline

**Contributors**  
Tysir Shehadey  
Jose Guarneros Padilla

