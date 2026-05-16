# Adult-income-prediction
An individual’s annual income results from various factors. Intuitively, it is influenced by the individual’s education level, age, gender, occupation, and etc.

Fields
The dataset contains 16 columns
Target filed: Income
-- The income is divide into two classes: <=50K and >50K
Number of attributes: 14
-- These are the demographics and other features to describe a person
# Feature Importance 
<img width="594" height="547" alt="تنزيل (1)" src="https://github.com/user-attachments/assets/8129eca9-8b71-42d6-82f7-1ebbe74fa95e" />
# Permutation importance
<img width="522" height="790" alt="تنزيل" src="https://github.com/user-attachments/assets/cfa60d76-63ea-4345-9b79-5dc44d36927d" />

# Model insight
“The bar plot indicates that the >50K income group has a higher average age than the <=50K group. This suggests that age may be positively related to income in this dataset, possibly because older individuals have more work experience and career progression.”
<img width="1104" height="649" alt="Screenshot 2026-05-07 114202" src="https://github.com/user-attachments/assets/228bace0-958f-4fc6-8211-d193d082c262" />


“The hours-per-week vs income plot shows that the >50K group has a higher average number of working hours per week than the <=50K group. This suggests that longer working hours may be associated with higher income in this dataset.”
<img width="1137" height="641" alt="image" src="https://github.com/user-attachments/assets/2c08c625-19ef-4e29-abea-8ca0ba1be0af" />


# Permutation importance after feature engineering and feature selection
<img width="1187" height="717" alt="image" src="https://github.com/user-attachments/assets/ca951340-7a5a-4b82-b262-fc33f1595234" />


## Feature Selection Using RFE

We applied Recursive Feature Elimination (RFE) using a Random Forest classifier to select the top 20 features from the dataset, including engineered features.

### Model Performance Comparison

- Baseline model accuracy: **[enter your result]**
- RFE model accuracy: **[enter your result]**

The RFE model reduces the number of features while maintaining or improving performance.

### Top 10 Important Features

Based on permutation importance, the top features are:

- [copy features from output]

### Comparison with Part 1

Compared to the original model from Part 1:

- Some key features such as **education, hours-per-week, and capital-gain** are still among the most important.
- New engineered features (such as **[your engineered features]**) appear in the top 10, showing that feature engineering added useful predictive information.

### Conclusion

Using RFE helped simplify the model by selecting the most relevant features, improving interpretability while keeping strong predictive performance.
