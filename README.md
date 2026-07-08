# Spotify Song Popularity Classification

## Overview

This project uses machine learning classification methods to predict whether a song will achieve high popularity based on audio characteristics and metadata from Spotify.

The goal of this project is to understand which musical features contribute most to song popularity and develop predictive models that can classify songs based on their likelihood of becoming popular.

This project applies statistical learning techniques to analyze patterns in music data and explore how measurable audio characteristics relate to audience engagement.

---

## Author

**James Ho**

**Course:** Data Science / Statistical Machine Learning  
**Institution:** Colorado State University

---

# Motivation

The music industry generates massive amounts of streaming data, making predictive analytics increasingly valuable for artists, producers, and streaming platforms.

Understanding why certain songs become popular can help answer questions such as:

- Which audio features are associated with successful songs?
- Can popularity be predicted using measurable song characteristics?
- How accurately can machine learning classify future popular songs?

This project applies classification algorithms to investigate the relationship between Spotify audio features and song popularity.

---

# Research Questions

This project investigates:

1. Can machine learning models accurately classify songs based on popularity?
2. Which Spotify audio features are most predictive of popularity?
3. How do different classification algorithms compare?
4. What characteristics separate popular songs from less popular songs?

---

# Dataset

The dataset consists of Spotify song information, including audio features and popularity metrics.

Each observation represents an individual song with variables such as:

## Audio Features

- Danceability
- Energy
- Loudness
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo
- Duration

## Metadata Features

- Artist information
- Genre information
- Release characteristics
- Popularity score

The target variable is a binary popularity classification:

\[
Y =
\begin{cases}
1, & \text{Popular Song}\\
0, & \text{Less Popular Song}
\end{cases}
\]

---

# Data Processing

The following preprocessing steps were performed:

1. Removed unnecessary variables.
2. Handled missing values.
3. Converted categorical variables into numerical features.
4. Created a binary popularity classification target.
5. Split data into training and testing sets.
6. Standardized numerical features when required by models.

---

# Exploratory Data Analysis

Initial analysis explored relationships between Spotify features and song popularity.

Analysis included:

- Distribution of popularity scores
- Feature correlations
- Comparison of audio characteristics between popular and less popular songs
- Feature importance analysis

Key questions explored:

- Are popular songs more energetic?
- Does danceability influence popularity?
- Are certain genres or characteristics associated with higher success?

---

# Machine Learning Models

Multiple classification models were developed and compared.

## Logistic Regression

A baseline classification model used to estimate the relationship between song features and popularity.

Advantages:

- Interpretable coefficients
- Provides insight into feature importance
- Establishes baseline performance

---

## Support Vector Machine (SVM)

A Support Vector Machine classifier was used to identify nonlinear patterns between Spotify features and song popularity.

Advantages:

- Effective in high-dimensional feature spaces
- Captures complex decision boundaries
- Provides strong classification performance

---

## Additional Classification Models

Other models were evaluated to compare predictive performance, including:

- Decision Trees
- Random Forest
- K-Nearest Neighbors

---

# Model Workflow

```
Spotify Dataset
        |
        v
Data Cleaning
        |
        v
Exploratory Data Analysis
        |
        v
Feature Engineering
        |
        v
Train/Test Split
        |
        v
Classification Models
        |
        v
Performance Evaluation
        |
        v
Popularity Prediction
```

---

# Model Evaluation

Models were evaluated using classification metrics:

## Accuracy

Measures overall prediction correctness.

\[
Accuracy =
\frac{Correct Predictions}{Total Predictions}
\]

---

## Precision

Measures how many songs predicted as popular were actually popular.

---

## Recall

Measures how many popular songs were successfully identified.

---

## F1 Score

Balances precision and recall.

\[
F1 =
2 \times
\frac{Precision \times Recall}
{Precision + Recall}
\]

---

## Confusion Matrix

Used to evaluate:

- Correct classifications
- False positives
- False negatives

---

# Results

The classification models demonstrated that Spotify audio characteristics contain meaningful information about song popularity.

Key findings:

- Audio features can provide predictive information about popularity.
- Some features contribute more strongly to classification than others.
- Machine learning models can identify patterns associated with successful songs.
- Model comparison reveals differences between interpretable and more complex algorithms.

---

# Feature Importance

Feature analysis was performed to identify characteristics most associated with popularity.

Important variables included:

- Energy
- Danceability
- Loudness
- Valence
- Tempo
- Acousticness
- Artist and metadata information

Understanding these relationships provides insight into measurable factors that influence streaming success.

---

# Repository Structure

```
Spotify-Popularity-Classification/
│
├── Data/
│   └── spotify_dataset.csv
│
├── Code/
│   ├── Data_Preprocessing.R
│   ├── EDA.R
│   ├── Classification_Models.R
│   └── Model_Evaluation.R
│
├── Figures/
│   ├── feature_distributions.png
│   ├── correlation_matrix.png
│   ├── confusion_matrix.png
│   └── feature_importance.png
│
├── Report/
│   └── Spotify_Popularity_Report.pdf
│
└── README.md
```

---

# Technologies Used

## Programming Languages

- R

## Libraries

- tidyverse
- caret
- ggplot2
- randomForest
- e1071
- dplyr

## Statistical and Machine Learning Methods

- Exploratory Data Analysis
- Feature Engineering
- Logistic Regression
- Support Vector Machines
- Random Forest
- Classification Metrics
- Model Comparison

---

# Future Improvements

Potential improvements include:

- Incorporating streaming count data over time
- Adding artist-level information
- Using deep learning approaches
- Applying natural language processing to lyrics
- Including playlist placement information
- Building a recommendation or hit prediction system

---

# Conclusion

This project demonstrates how statistical learning methods can be applied to music analytics by predicting song popularity from Spotify features.

Through exploratory analysis, feature engineering, and classification modeling, the project provides insight into the measurable characteristics associated with successful songs and highlights the role of machine learning in understanding modern music trends.
