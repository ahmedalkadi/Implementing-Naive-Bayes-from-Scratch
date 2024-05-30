# Implementing Naive Bayes from Scratch for IMDB Fake / Real Review Classification

## Introduction
Bayes Theorem is named after the English mathematician Thomas Bayes, who made significant contributions to decision theory, a field of mathematics that involves probabilities. Bayes Theorem is widely used in machine learning as a simple and effective way to predict classes with precision and accuracy. The Bayesian method of calculating conditional probabilities is particularly useful in classification tasks.

This project focuses on implementing the Naive Bayes classification algorithm from scratch to classify IMDB reviews as fake or real. Specifically, we will implement the Multinomial Naive Bayes classifier, which is well-suited for text classification tasks where the features are word frequencies or counts.

## Naive Bayes Theorem

### Bayes Theorem Theory
Bayes Theorem is expressed as:

$$
P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}
$$

Where:
- \( P(A|B) \) is the posterior probability: the probability of hypothesis \( A \) given the data \( B \).
- \( P(B|A) \) is the likelihood: the probability of data \( B \) given that hypothesis \( A \) is true.
- \( P(A) \) is the prior probability: the initial probability of hypothesis \( A \).
- \( P(B) \) is the marginal probability: the total probability of data \( B \).

### Naive Bayes Classification
The Naive Bayes classifier simplifies Bayes Theorem by assuming that the features are independent given the class label. The formula for Naive Bayes is:

$$
P(C|x_1, x_2, \ldots, x_n) \propto P(C) \prod_{i=1}^n P(x_i|C)
$$

Where:
- \( P(C|x_1, x_2, \ldots, x_n) \) is the probability of class \( C \) given the features \( x_1, x_2, \ldots, x_n \).
- \( P(C) \) is the prior probability of class \( C \).
- \( P(x_i|C) \) is the likelihood of feature \( x_i \) given class \( C \).

