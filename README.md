# Performance_Metrics

1.	Accuracy:
* Formula: (TP + TN) / (TP + TN + FP + FN)
* Example: Predicting whether an email is spam (binary classification).
* Use Case: Balanced datasets with roughly equal class distribution.
* Not Ideal For: Imbalanced datasets where one class is much more frequent.
2.	Precision:
* Formula: TP / (TP + FP)
* Example: Medical diagnosis to minimize false positives (e.g., disease detection).
* Use Case: When avoiding false positives is crucial.
* Not Ideal For: When false negatives have severe consequences.
3.	Recall (Sensitivity):
* Formula: TP / (TP + FN)
* Example: Identifying fraudulent transactions to minimize false negatives.
* Use Case: When avoiding false negatives is critical.
* Not Ideal For: When false positives are more acceptable.
4.	F1-Score:
* Formula: 2 * (Precision * Recall) / (Precision + Recall)
* Example: Information retrieval, where both precision and recall are important.
* Use Case: Balancing precision and recall in tasks like document retrieval.
* Not Ideal For: Situations heavily favoring one metric over the other.
5.	Specificity:
* Formula: TN / (TN + FP)
* Example: Medical tests to correctly identify healthy individuals.
* Use Case: When true negatives are of interest.
* Not Ideal For: Situations where false positives are more significant.
6.	ROC-AUC:
* Formula: Area under the Receiver Operating Characteristic curve.
* Example: Evaluating a model's ability to discriminate between classes.
* Use Case: Comparing models with different thresholds or class distributions.
* Not Ideal For: Imbalanced datasets or when ranking isn't relevant.
7.	Mean Absolute Error (MAE):
* Formula: (1/n) * Σ|actual - predicted|
* Example: Predicting house prices.
* Use Case: When the magnitude of errors matters.
* Not Ideal For: When outliers heavily affect performance.
8.	Mean Squared Error (MSE):
* Formula: (1/n) * Σ(actual - predicted)^2
* Example: Regression tasks like predicting stock prices.
* Use Case: When larger errors should be penalized more.
* Not Ideal For: Sensitive to outliers; squared errors can amplify them.
9.	Mean Squared Logarithmic Error (MSLE):
* Formula: (1/n) * Σ(log(1 + actual) - log(1 + predicted))^2
* Example: Forecasting tasks where relative errors are more important.
* Use Case: When predicting values that can have a wide range of magnitudes.
* Not Ideal For: Cases where small errors matter less.
10.	Root Mean Squared Error (RMSE):
* Formula: √((1/n) * Σ(actual - predicted)^2)
* Example: Regression tasks similar to MSE.
* Use Case: When you want the error metric in the same unit as the target variable.
* Not Ideal For: Sensitive to outliers, similar to MSE.
11.	Mean Percentage Error (MPE):
* Formula: (1/n) * Σ((actual - predicted) / actual) * 100
* Example: Sales forecasting, demand prediction.
* Use Case: When you want to express errors as percentages.
* Not Ideal For: Prone to division by zero if actual values are zero.
12.	Mean Absolute Percentage Error (MAPE):
* Formula: (1/n) * Σ|((actual - predicted) / actual)| * 100
* Example: Financial forecasting, inventory management.
* Use Case: Expressing errors as percentages with less bias towards larger errors.
* Not Ideal For: Division by zero if actual values are zero; not symmetric.
13.	Cohen's Kappa:
* Formula: (Po - Pe) / (1 - Pe)
* Example: Evaluating inter-rater agreement.
* Use Case: When dealing with imbalanced classes or subjective judgments.
* Not Ideal For: Inappropriate for multiclass problems; can be sensitive to class distribution.
14.	Matthews Correlation Coefficient (MCC):
* Formula: (TP * TN - FP * FN) / √((TP + FP) * (TP + FN) * (TN + FP) * (TN + FN))
* Example: Binary classification tasks.
* Use Case: Handling imbalanced datasets and multiclass problems.
* Not Ideal For: In multiclass problems, some variants like balanced MCC may be preferred.
15.	Adjusted Rand Index (ARI):
* Formula: (RI - Expected_RI) / (max(RI) - Expected_RI)
* Example: Clustering evaluation.
* Use Case: Assessing the similarity between true and predicted clusters.
* Not Ideal For: Random clusterings can lead to non-zero scores.
16.	Log Loss (Cross-Entropy Loss):
* Formula: -(1/n) * Σ(actual * log(predicted) + (1 - actual) * log(1 - predicted))
* Example: Binary classification, probabilistic predictions.
* Use Case: When predicting probabilities; penalizes confident wrong predictions.
* Not Ideal For: Not suitable for non-probabilistic tasks


