# Amazon Echo Rating Review Predictor

## Overview
This project focuses on predicting Amazon Echo product ratings based on customer reviews. Utilizing a dataset comprising over 50,000 Amazon Echo reviews, each paired with a corresponding rating ranging from 1 to 5, I embarked on a comprehensive analysis to derive meaningful insights and build predictive models.

Due to computational constraints, our analysis is based on a subset of 5,000 selected reviews.

## Data Preprocessing and Embedding
The textual content of the reviews was embedded using various text embedding models, including:
- OpenAI's Ada Text Embedder
- Roberta-base
- A Roberta base variant
- MiniLM

The detailed procedures for each embedding technique are  documented in the respective Jupyter notebooks provided in the project repository.

## Modeling and Analysis
Our approach to predicting the product ratings involved both regression and classification models.

### Regression
I initially applied regression models to predict the ratings, experimenting with:
- Linear Regression
- Random Forest Regression
- XGBoost Regression

The Random Forest Regression model, particularly when used in conjunction with OpenAI embeddings, emerged as the best performer. Detailed results and analyses are available in the regression notebook. The model exhibited proficiency in distinguishing between extreme ratings (1 and 5), but faced challenges with intermediate ratings (2, 3, and 4) due to the textual similarities in the reviews.

### Classification
To enhance our predictive accuracy, I transitioned to classification models, specifically employing Random Forest Classification. The results were showed slight improvements over the regression models.

Further refinement was achieved by consolidating the rating classes, leading to better model performance. All findings and  analyses pertaining to the classification models can be found in the classification notebook.

## Data and Notebooks
Due to the substantial size of certain CSV files, I opted to exclude them from the repository. However, a selection of files has been retained to provide context and illustrate the structure of the data used in the analyses.

## Conclusion
This project shows the challenges and nuances of predicting product ratings based on textual reviews. While the models demonstrated competence in distinguishing between distinctly positive and negative reviews, the subtleties of intermediate ratings pose a significant challenge, highlighting the need for advanced modeling techniques and feature engineering to further enhance predictive accuracy.
