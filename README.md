# Goal Prediction and Player Performance Analytics

This project leverages **Machine Learning** and **Data Analytics** to predict football match outcomes, focusing on goal prediction and player performance analysis. Using a dataset of over 900,000 events across European football leagues, the model predicts the likelihood of a goal based on various match and player conditions.

## Project Overview

The goal of this project is twofold:
1. **Predict Goal Likelihood**: Develop a model to estimate the probability of scoring based on match-specific features.
2. **Player Performance Metrics**: Establish benchmarks for player performance using a standardized metric, isolating skill by removing luck and contextual factors.

## Methodology

1. **Dataset Selection**: The dataset from Kaggle includes events from 9,074 matches across major European leagues. Key files include:
   - `events.csv`: Detailed event data.
   - `ginf.csv`: Metadata and match odds.
   - `dictionary.txt`: Dictionary of event types.

2. **Data Processing**:
   - **Cleaning**: Filtered and removed null values from critical fields.
   - **Feature Selection**: Selected relevant features, including `time`, `location`, `situation`, etc., for predictive modeling.

3. **Modeling**:
   - Trained multiple ML models (e.g., Gradient Boosting, Random Forest) on both encoded and non-encoded feature sets.
   - Achieved best performance with **Gradient Boosting Classifier**, achieving over 90% accuracy.

4. **Player Metric Development**:
   - Derived several performance metrics, including `xG_diff` (goals scored vs. predicted goals), `xG_per_shot`, and counter-attacking ability, providing a structured assessment of player effectiveness.

## Results

- **Goal Prediction Accuracy**: The model reliably predicts goal-scoring chances with 91% accuracy, assisting teams in decision-making.
- **Player Performance Analysis**: Custom metrics allow coaches and analysts to gauge a player’s skill independently of external factors, focusing on their unique scoring potential.

## Conclusion

This project successfully demonstrates the potential of machine learning in sports analytics by predicting outcomes and creating insightful player metrics. Future work could expand on these models by incorporating additional player attributes, commentary data, and advanced NLP techniques.

## Requirements

- Python (version 3.x)
- Libraries: scikit-learn, pandas, numpy, matplotlib, seaborn

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/slenka28/Goal-Prediction-and-Player-Performance-Analytics.git
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the data preprocessing and model training scripts to generate predictions and player metrics.

## License

This project is open-source and available under the MIT License.
