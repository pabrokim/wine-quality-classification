
**Wine Quality Classification with Logistic Regression**
This project explores the use of Logistic Regression to predict wine quality based on a set of physicochemical features. Using a dataset of white wines, a binary classifier was trained that distinguished between lower and higher quality wines.

**Motivation**
Wine quality is a complex attribute influenced by a blend of chemical properties. By applying machine learning, particularly logistic regression, the project aimed to understand which features contributed most to a wine’s perceived quality—and to predict that quality with reasonable accuracy.The goal was to build a logistic regression model that predicts whether a wine is of good quality or not, using features like acidity, alcohol, pH, and more.

**Model Performance**
Once the dataset was cleaned, and model trained on a standard training/testing split, it performed as follows:
Baseline Accuracy (majority class): 0.79
Training Accuracy: 0.81
Testing Accuracy: 0.78

The model slightly outperformed the baseline, showing its capacity to learn meaningful patterns in the data.

**Key Feature Insights (Model Coefficients)**

Logistic regression gave interpretable coefficients that indicate the influence of each feature on the prediction.
Feature	Coefficient	Interpretation
Volatile Acidity	-3.06	Higher levels strongly decrease quality
Chlorides	-1.33	Negatively impacts quality
Citric Acid	-0.70	Slightly lowers quality
Total Sulfur Dioxide	0.001	Minimal effect
Fixed Acidity	0.005	Minimal positive effect
pH	0.79	Higher pH slightly increases quality
Alcohol	0.84	Strong positive influence
Sulphates	1.04	Most positively correlated with quality
Therefore, white wines with higher alcohol and sulphate levels are more likely to be of good quality, while high volatile acidity significantly reduces quality perception.

**Confusion Matrix**
To further evaluate the model, a confusion matrix on the test set was implemented and revealed the following:
True Positives (TP): 54 wines correctly classified as high quality
True Negatives (TN): 715 wines correctly identified as low quality
False Negatives (FN): 173 wines incorrectly labeled as good
False Positives (FP): 38 good-quality wines missed

Evidently, the model performs well on identifying low quality wines suggesting bias in predicting not good.

**Conclusion**
Logistic Regression provided a transparent and interpretable model for wine quality prediction. While simple, it highlighted key chemical drivers of quality—particularly alcohol content, sulphates, and volatile acidity. 