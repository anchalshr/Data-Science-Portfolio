## Objective of this project:
To build an ML model to predict the sentiment of the review text.

## Dataset
In this dataset, each record represents a movie-review pair with movie title, description, genres, duration, 
director, actors, users' ratings, review text, reviewer name, etc.

## Data Files
train.csv - the training set containing the review sentiment along with other features.
test.csv - the test set has review features, but no sentiment column, since it is the target.
movies.csv - the file with metadata on movies.
Column named "sentiment" - indicating "POSITIVE" or "NEGATIVE", which is the target.

## Methodology
Exploratory Data Analysis (EDA)
1. Dataset structure and data types were examined using .info().
2. A correlation matrix was plotted to understand relationships between numerical variables.
3. A count plot was generated to analyze sentiment class distribution.
4. Missing values were handled using simple imputation (replacing null values with empty strings).

Three classification models were implemented using Scikit-learn Pipelines:
1. Logistic Regression (LogisticRegressionCV): Used cross-validation for hyperparameter tuning, Integrated with preprocessing steps using a pipeline.
2. Decision Tree Classifier: Built with random_state=0. Tree visualization performed to inspect decision structure (limited depth for clarity).
3. Multinomial Naive Bayes: Suitable for text classification problems. Trained using TF-IDF features.

## Results
1. The sentiment distribution analysis showed the class balance across categories.
2. Text-based feature engineering using TF-IDF significantly improved model performance.
3. Among the three models, Logistic Regression achieved the highest accuracy and demonstrated better generalization.
