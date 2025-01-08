# Analysis and Prediction of Student Graduates

This project arose from an academic assignment of "Maestría en Explotación de Datos y Descubrimiento del Conocimiento" (Master’s in Data Mining and Knowledge Discovery), Universidad de Buenos Aires (UBA), in which we were asked to use various machine learning models to predict whether university students would complete their studies. The main objective was to measure performance when using multiple models to handle the target.

## Project Description

This analysis focuses on applying multiple machine learning algorithms to predict **student dropout** at universities. Various techniques were implemented to ensure model robustness, including splitting into **training and test sets**, as well as the use of **cross-validation** for hyperparameter optimization.

Different metrics were used to evaluate the models’ performance on both training and test data, along with **complexity curves** and **optimization techniques**. This allowed for a precise and detailed evaluation of the performance of each model.

## Models and Results

- For predicting the **binary target** (whether a student will complete the degree or not), the best performance was achieved with **Logistic Regression**.
- For predicting **multiclass variables** (types of dropout), the most effective model was the **Decision Tree**.
- Additionally, **ensemble** techniques were implemented, using models like **AdaBoost** and **Bagging KNeighborsClassifier**, which significantly improved performance in some cases .

## Data Set Analysis

The project was based on a provided dataset, which underwent thorough **exploratory analysis** and **preprocessing** before applying machine learning models. Techniques such as **One-Hot Encoding** were used for categorical variables, and **StratifiedKFold** was employed to ensure correct data partitioning during validation.

## Evaluation Metrics

The metrics used to evaluate model performance were:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC AUC**
- **Log Loss**

These metrics enabled a comprehensive evaluation of model performance, ensuring that not only accuracy was maximized, but also other important aspects like the model’s ability to handle data imbalances.

## Techniques and Algorithms Used

- **Cross-Validation**: **StratifiedKFold** (5 folds) was used to ensure proper segmentation of the training data.
- **One-Hot Encoding**: For categorical variables with more than two levels.
- **Algorithms**: Models such as **Logistic Regression**, **Support Vector Machine (SVM)**, **Decision Trees (CART)**, and **K-Nearest Neighbors (KNN)** were used for both binary and multiclass prediction.
- **Multiclass Classification**: **OneVsRestClassifier (OVRC)** and **OneVsOneClassifier (OVOC)** were implemented for multiclass classification problems.
- **Ensemble Techniques**: **Bagging** (ensemble-KNN) and **Boosting** (AdaBoost) models were applied.
