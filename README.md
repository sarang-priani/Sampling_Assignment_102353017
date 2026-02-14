# Sampling Assignment – Credit Card Fraud Detection

**Name:** Sarang Priani  
**Roll No:** 102353017  

---

## Objective
The objective of this assignment is to analyze the effect of different sampling techniques on machine learning model performance using an imbalanced credit card fraud dataset. The experiment evaluates how balancing the dataset and applying probabilistic sampling techniques influence classification accuracy.

---

## Dataset
Dataset Link:  
https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv  

The dataset contains credit card transactions classified as:
- Class 0 → Non-Fraud  
- Class 1 → Fraud  

The dataset is highly imbalanced.

---

## Data Balancing
The dataset was first divided into training and testing sets.  
Random Over Sampling was applied to the training data to convert it into a balanced class dataset.  
This ensures that both classes are equally represented during model training.

---

## Sampling Techniques Used
After balancing, five probabilistic sampling techniques were applied:

1. Sampling1 – Simple Random Sampling  
2. Sampling2 – Systematic Sampling  
3. Sampling3 – Stratified Sampling  
4. Sampling4 – Cluster Sampling  
5. Sampling5 – Bootstrap Sampling  

---

## Machine Learning Models Used

- M1 – Logistic Regression  
- M2 – Support Vector Machine (SVM)  
- M3 – K-Nearest Neighbors (KNN)  
- M4 – Decision Tree  
- M5 – Naive Bayes  

---

## Accuracy Results

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|-------|-----------|-----------|-----------|-----------|-----------|
| M1 | 95.03 | 92.59 | 96.89 | 96.30 | 94.67 |
| M2 | 98.76 | 95.06 | 98.76 | 98.77 | 98.67 |
| M3 | 93.17 | 88.89 | 96.89 | 92.59 | 94.67 |
| M4 | 97.52 | 95.06 | 97.52 | 98.77 | 92.89 |
| M5 | 78.88 | 75.31 | 77.02 | 80.25 | 76.89 |

---

## Best Performing Combination

- **Model:** M2 (SVM)  
- **Sampling Technique:** Sampling4 (Cluster Sampling)  
- **Accuracy:** 98.77 %

---

## Screenshot 1 – Accuracy Table and result
<img width="1246" height="582" alt="image" src="https://github.com/user-attachments/assets/805bfba8-e972-4fdb-8daf-2ab6f18dfc58" />


---

## Screenshot 2 – Accuracy Comparison Graph
<img width="1694" height="1112" alt="image" src="https://github.com/user-attachments/assets/369cbeec-0570-4a5b-802c-1f6cdb2b1176" />


---

## Discussion
The dataset was initially highly imbalanced, which can negatively affect classification performance. Random Over Sampling was used to balance the training data before applying probabilistic sampling techniques.

The results show that model performance varies depending on the sampling method used. SVM (M2) achieved the highest accuracy under Cluster Sampling. Naive Bayes showed comparatively lower performance due to its strong independence assumption. Overall, sampling strategy plays an important role in influencing classification accuracy.

---

## Conclusion
Balancing the dataset significantly improved model performance. Different sampling techniques produced varying accuracy results across models. The experiment demonstrates the importance of proper sampling and preprocessing when handling imbalanced datasets.
