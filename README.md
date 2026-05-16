# Adult-income-prediction

An individual’s annual income is influenced by various factors. Intuitively, it depends on characteristics such as education level, age, gender, occupation, and others.

### Fields

The dataset contains **16 columns**.

* **Target field:** Income
  * The income is divided into two classes: **<=50K** and **>50K**

* **Number of attributes:** 14
  * These represent demographic and other characteristics used to describe an individual.


### Top 10 Permutation Important Features

- **Baseline Model**
 <img width="522" height="790" alt="تنزيل" src="https://github.com/user-attachments/assets/cfa60d76-63ea-4345-9b79-5dc44d36927d" />
 
- # Feature Importance 
<img width="594" height="547" alt="تنزيل (1)" src="https://github.com/user-attachments/assets/8129eca9-8b71-42d6-82f7-1ebbe74fa95e" />
 
- **Feature Eng + RFE**
  <img width="1187" height="717" alt="image" src="https://github.com/user-attachments/assets/ca951340-7a5a-4b82-b262-fc33f1595234" />

## ✅ Overall Comparison

| Model                   | Accuracy   | Precision (>50K) | Recall (>50K) | F1-score (>50K) | Time        |
| ----------------------- | ---------- | ---------------- | ------------- | --------------- | ----------- |
| **Baseline Model**      | ✅ **0.86** | **0.73**         | 0.64          | 0.68            | Fast        |
| **PCA Model**           | 0.79       | 0.53             | ✅ **0.79**    | 0.64            | 12.33 sec   |
| **Feature Engineering** | 0.85       | 0.67             | 0.71          | 0.69            | ✅ 10.65 sec |
| **Feature Eng + RFE**   | 0.85       | 0.67             | 0.72          | 0.69            | Slowest     |



### Conclusion

While the baseline model achieved the highest accuracy, feature engineering provided a better balance between performance and recall for the >50K class. PCA reduced model performance significantly, while RFE increased computation time without meaningful improvement. Therefore, the feature engineering model offers the best practical trade-off between accuracy, efficiency, and interpretability.
