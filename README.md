# Naive Bayes Classifier Comparison on Twitter Sentiment Analysis

## Overview

This project compares the performance of four different Naive Bayes algorithms on a given dataset. The algorithms evaluated include Multinomial Naive Bayes, Bernoulli Naive Bayes, Complement Naive Bayes, and Gaussian Naive Bayes.

## Naive Bayes Algorithms

### Multinomial Naive Bayes

- Accuracy: 94.40%
- Multinomial Naive Bayes is suitable for discrete data, often used in text classification tasks where the features represent the frequency of words or other discrete data. It assumes that the features are generated from a multinomial distribution and is particularly effective when dealing with data that can be modeled as counts.

### Bernoulli Naive Bayes

- Accuracy: 94.34%
- Bernoulli Naive Bayes is designed for binary and categorical features, commonly used in text classification and spam filtering. It models the presence or absence of each feature and assumes that each feature is conditionally independent, given the class label. It is effective when dealing with binary features.

### Complement Naive Bayes

- Accuracy: 89.43%
- Complement Naive Bayes is an adaptation of the standard Multinomial Naive Bayes algorithm. It is designed to handle imbalanced datasets, where some classes have significantly more instances than others. It complements the standard Multinomial Naive Bayes by adjusting the class priors during training to give more weight to the minority class.

### Gaussian Naive Bayes

- Accuracy: 46.11%
- Gaussian Naive Bayes is suitable for continuous data and assumes that the features are normally distributed within each class. It is commonly used when dealing with real-valued features. However, it makes the simplifying assumption that the features are uncorrelated within each class and may not perform well if this assumption is violated

## Results and Discussion

# Results and Discussion

## Complement Naive Bayes

The Complement Naive Bayes model achieved an accuracy of 89.43%. The confusion matrix reveals that the model performed well in correctly predicting the majority class (0), but struggled with the minority class (1). The classification report highlights the imbalance, with a notable difference in precision, recall, and F1-score between the two classes. The weighted average F1-score is 0.90, indicating a good overall performance, but attention is needed to improve the model's handling of the minority class.

## Multinomial Naive Bayes

The Multinomial Naive Bayes model exhibited a higher accuracy of 94.40%. It demonstrated excellent performance in predicting the majority class (0) with a high precision and recall. However, the model struggled with the minority class (1), as reflected in the lower precision, recall, and F1-score for that class. The weighted average F1-score is 0.93, suggesting a strong overall performance but with room for improvement, particularly in addressing imbalances.

## Bernoulli Naive Bayes

The Bernoulli Naive Bayes model achieved an accuracy of 94.34%. Similar to the Multinomial model, it excelled in predicting the majority class (0) but faced challenges in accurately predicting the minority class (1). The confusion matrix and classification report reveal patterns consistent with imbalanced datasets. The weighted average F1-score is 0.93, indicating good overall performance, though efforts could be directed towards improving predictions for the minority class.

## General Discussion

All three Naive Bayes models demonstrated competitive accuracy, with Multinomial Naive Bayes slightly outperforming the others. However, it is crucial to consider the specific requirements of the application. If handling imbalanced data is a priority, techniques such as oversampling or using specialized algorithms like Complement Naive Bayes might be beneficial. Additionally, further tuning and exploration of hyperparameters could enhance the models' ability to generalize well to new data.

Understanding the strengths and weaknesses of each model is essential for making informed decisions based on the specific characteristics of the dataset and the goals of the application.


## Future Work

Discuss potential improvements or further experiments that could be conducted to enhance the performance of the models. This could include hyperparameter tuning, feature engineering, or trying different algorithms.



