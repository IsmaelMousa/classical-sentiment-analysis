# Classical Sentiment Analysis

Develop a classical machine learning sentiment classifier for movie reviews.

[![Report](https://img.shields.io/badge/W&B_Full_Report-gray?logo=weightsandbiases&logoColor=yellow)](https://api.wandb.ai/links/research-devellopment/hjgmo1ka)


## Introduction

This project aims to build an optimal sentiment analysis model using classical machine learning techniques to classify
movie reviews as positive or negative. The model's performance will be primarily evaluated using the f1-score.

## Methodology

**Nine Experiments** were conducted to evaluate different preprocessing techniques, model architectures, and
hyperparameter settings. The dataset consists of annotated movie reviews labeled as pos (positive) and neg (
negative). The following steps outline the approach:

#### Data Analysis

- Exploration of class distribution to ensure balanced representation.
- Examination of word frequency and sentiment-based patterns.
- Visualization of key terms using statistical summaries.

#### Data Preprocessing

- Text cleaning: removal of punctuation, stopwords, and special characters.
- Tokenization and lemmatization for feature standardization.
- Transformation using TF-IDF vectorization to represent text numerically.

#### Model Configuration

- Implementation of Naïve Bayes, Logistic Regression, and Random Forests.
- Experimentation with different vectorization and model settings.

#### Evaluation

- Performance assessment using train/test: loss, accuracy, f1-score, precision, and recall.
- Analysis of confusion matrices to evaluate classification errors and model reliability.
- Comparison of models to determine the most effective approach.

#### Tracking

- Experiment tracking and visualization
  using [Weights & Biases (W&B)](https://api.wandb.ai/links/research-devellopment/hjgmo1ka).
- Logging configurations, hyperparameters, performance metrics, and training history.
- Comparing runs to identify the best-performing configurations.

## Results

- Naïve Bayes: performed well, trailing behind Logistic Regression, but still demonstrated strong
  classification ability.
- Random Forests: showed the lowest performance among the three models, the decreased accuracy and F1-score suggest
  overfitting, as the model might have been too complex for the dataset.
- Logistic Regression: achieved the highest performance across all metrics, making it the most effective model for
  our task.

#### Table below summarizes the best test performance metrics achieved by each model

|           Model           |  Accuracy  |  F1-Score  | Precision  |   Recall   |   Loss   |
|:-------------------------:|:----------:|:----------:|:----------:|:----------:|:--------:|
|      **Naïve Bayes**      |   82.78%   |   82.47%   |   84.42%   |   82.48%   |   0.50   |
|    **Random Forests**     |   80.66%   |   80.45%   |   81.48%   |   80.44%   |   0.53   |
|  **Logistic Regression**  | **88.22%** | **88.18%** | **88.36%** | **88.13%** | **0.49** |


## Conclusion

This project evaluates the performance of three classical machine learning algorithms: Logistic Regression, Naïve Bayes, and Random Forest on a sentiment analysis task. 

The **9th experiment** achieved the highest performance. Key to the success of the models were the feature engineering and data preprocessing strategies employed.
