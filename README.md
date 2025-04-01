# IPL Runs Prediction Model

This project predicts whether a cricket team will score 30 or more runs in the first 3 overs of an IPL match. The model is built using historical IPL data and incorporates features such as team performance, venue conditions, and bowling team statistics to make predictions.

## Project Overview

The model uses various features including:

- **Average runs scored by the batting team in the first 3 overs**.
- **Average runs conceded by the bowling team in the first 3 overs**.
- **Average runs scored at the venue**.

Using these features, a logistic regression model predicts whether the batting team will score 30 or more runs in the first 3 overs.

## Requirements

- Python 3.x
- pandas
- scikit-learn
- joblib

## Installation

Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/your-username/ipl-runs-prediction.git
cd ipl-runs-prediction
pip install -r requirements.txt
run ipl.ipynb

```
## Data
The dataset used in this project is IPL match data, which contains information about:

Match details (match_id, batting_team, bowling_team, venue).

Performance data (runs_batter, runs_extras, over).

The dataset is expected to be in a CSV format named IPL.csv.

## Model Explanation
Data Preprocessing:

Filter the data to include only the first 3 overs.

Calculate the total runs scored in the first 3 overs by summing runs scored by the batter and extras.

## Feature Engineering:

Calculate average runs scored by each team in the first 3 overs.

Calculate average runs conceded by each bowling team.

Calculate average runs scored at each venue.

## Model Training:

A logistic regression model is trained to predict whether a team will score 30 or more runs in the first 3 overs.

## Model Evaluation:

The model is evaluated using accuracy and classification report metrics.

## Results
The model provides predictions on whether a team will score 30+ runs in the first 3 overs based on historical data. The predictions are made with an accuracy that is evaluated using the classification report.
