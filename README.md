# League of Legends 10-Minute Match Outcome Prediction

This project is part of the Miuul Bootcamp and aims to predict the outcome of a League of Legends (LoL) match within the first 10 minutes using machine learning models implemented in Python. The primary model utilized is a Voting Classifier composed of various base models that have been fine-tuned to provide the best prediction accuracy. The project includes data preprocessing, exploratory data analysis, model building, and deployment using Streamlit.

## Project Files

- `datasets/high_diamond_ranked_10min.csv`: The dataset used for training and testing the model, consisting of features collected from high-ranked matches within the first 10 minutes.
- `icon.png`: Icon used in the Streamlit web application.
- `lol_cover.jpg`: Cover image used in the Streamlit web application.
- `lol_prediction.joblib`: The trained model file, saved using Joblib for later use in predictions.
- `required_functions.py`: A Python script containing custom functions used throughout the project for data preprocessing and evaluation.
- `requirements.txt`: A list of Python packages required to run the project.
- `lol_10_min_prediction.py`: The main script that includes data preprocessing, model training, and evaluation steps.
- `main.py`: The script for deploying the web application using Streamlit, allowing users to input match data and receive predictions.

## Project Overview

League of Legends is a popular online multiplayer game where teams of five players each aim to destroy the opponent's base. This project focuses on predicting which team will win based on data from the first 10 minutes of gameplay. The project uses a combination of data science and machine learning techniques to create a predictive model that can estimate the likelihood of a team's victory early in the game.

### Data Preprocessing

The dataset undergoes extensive preprocessing, including:

- Dropping irrelevant or redundant features.
- Handling missing values and outliers.
- Feature scaling and encoding.

### Model Training

The model training process involves:

- Splitting the dataset into training and testing sets.
- Utilizing a Voting Classifier that combines the strengths of multiple machine learning models.
- Hyperparameter optimization to fine-tune the models.

### Model Evaluation

The model is evaluated based on various metrics such as accuracy, F1 score, and ROC AUC score. These metrics help in understanding the performance of the model in predicting match outcomes.

### Deployment

The project is deployed as a web application using Streamlit, allowing users to:

- View the dataset and perform exploratory data analysis.
- Input match details and receive a prediction on which team is likely to win.

## Installation

To run the project, you'll need to install the required dependencies listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

## Usage

1. **Run the Prediction Script**: 
   ```bash
   python lol_10_min_prediction.py
   ```
   This script will train the model and save it as `lol_prediction.joblib`.

2. **Deploy the Web Application**: 
   ```bash
   streamlit run main.py
   ```
   This will launch the web app where you can interact with the model and visualize the data.

## Conclusion

This project demonstrates the application of machine learning to real-world gaming data, providing insights into how early-game actions in League of Legends can influence the final outcome. The model's predictions can help players and analysts understand key factors that contribute to winning or losing a match.

## License

This project is licensed under the MIT License.
