
# Exoplanet Exploration

![exoplanets.jpg](exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

The machine learning models in this jupyter notebook can classify candidate exoplanets from the raw dataset.

## Compare Basic ML Models

![compareMLModels.png](compareMLModels.png)

## RandomForestClassifier

Training Data Score: 0.8411100945410186
Testing Data Score: 0.8403476669716377

                precision    recall  f1-score   support

     CANDIDATE       0.83      0.51      0.63       529
     CONFIRMED       0.74      0.85      0.79       568
FALSE-POSITIVE       0.90      0.99      0.94      1089
      accuracy       -          -        0.84      2186
     macro-avg       0.82      0.79      0.79      2186
  weighted-avg       0.84      0.84      0.83      2186


===========================================================
# LinearSVC

Training Data Score: 0.8595608417200366
Testing Data Score: 0.8513266239707228

                precision    recall  f1-score   support

     CANDIDATE       0.77      0.58      0.66       529
     CONFIRMED       0.69      0.82      0.75       568
  FALSE-POSITIVE     0.98      1.00      0.99      1089
      accuracy        -         -        0.85      2186
     macro-avg       0.81      0.80      0.80      2186
   weighted-avg      0.85      0.85      0.85      2186


===========================================================
# MultinomialNB

Training Data Score: 0.812137846904544
Testing Data Score: 0.8087831655992681

                precision    recall  f1-score   support

     CANDIDATE       0.84      0.29      0.43       529
     CONFIRMED       0.59      0.93      0.72       568
FALSE POSITIVE       0.98      1.00      0.99      1089
      accuracy        -         -        0.81      2186
     macro avg       0.80      0.74      0.71      2186
  weighted avg       0.84      0.81      0.78      2186


===========================================================
# LogisticRegression

Training Data Score: 0.845684659957304
Testing Data Score: 0.8371454711802379

                precision    recall  f1-score   support

     CANDIDATE       0.73      0.56      0.63       529
     CONFIRMED       0.67      0.79      0.72       568
FALSE POSITIVE       0.98      1.00      0.99      1089
      accuracy       -         -         0.84      2186
     macro avg       0.79      0.78      0.78      2186
  weighted avg       0.84      0.84      0.83      2186


===========================================================
SVC
                precision    recall  f1-score   support

     CANDIDATE       0.78      0.55      0.64       529
     CONFIRMED       0.67      0.84      0.75       568
FALSE POSITIVE       0.98      1.00      0.99      1089
      accuracy        -          -       0.85      2186
     macro avg       0.81      0.79      0.79      2186
  weighted avg       0.85      0.85      0.84      2186

Training Data Score: 0.8508691674290942
Testing Data Score: 0.8472095150960659
===========================================================

# Compare GridSearch Models
- - -
### GridSearchCV Model with a linear kernel:

#                 precision    recall  f1-score   support

     CANDIDATE       0.85      0.69      0.76       529
     CONFIRMED       0.76      0.87      0.81       568
FALSE POSITIVE       0.98      1.00      0.99      1089
      accuracy         -         -       0.89      2186
     macro avg       0.86      0.85      0.85      2186
  weighted avg       0.89      0.89      0.89      2186

### GridSearchCV Model with an rbf  kernel:

               precision    recall  f1-score   support

     CANDIDATE       0.84      0.71      0.77       529
     CONFIRMED       0.77      0.85      0.81       568
FALSE POSITIVE       0.98      1.00      0.99      1089
      accuracy        -         -        0.89      2186
     macro avg       0.86      0.85      0.86      2186
  weighted avg       0.89      0.89      0.89      2186


## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

- - -
