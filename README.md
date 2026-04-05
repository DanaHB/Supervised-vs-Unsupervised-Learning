# Machine Learning: Supervised vs. Unsupervised Evaluation
### Performance Analysis on Breast Cancer and Adult Income Datasets

## 1. Project Overview
This project evaluates the performance of different machine learning models using two datasets: **Breast Cancer Wisconsin** and **Adult Income**. The goal is to implement and compare supervised models (SVM, Logistic Regression, Naive Bayes) and unsupervised models (K-Means, Hierarchical Clustering) to see how they handle different data characteristics.

## 2. Methodology
The implementation follows a practical data science workflow:
* **Data Preprocessing:** Handled missing values and performed categorical encoding.
* **Data Scaling:** Applied **Normalization (Min-Max Scaling)** to ensure all features are on the same scale, which is essential for models that calculate distances.
* **Model Building:** * **Supervised:** Trained SVM, Logistic Regression, and Naive Bayes for classification.
* **Unsupervised:** Applied K-Means and Hierarchical Clustering to find natural groups in the data.


## 3. Discussion & Key Observations
* **Best Models:** **SVM** and **Logistic Regression** are recommended as they achieved the most reliable and highest performance across both datasets.
* **Naive Bayes Performance:** The Gaussian Naive Bayes struggled because it assumes a **Normal distribution**.
* **Importance of Preprocessing:** Scaling was a mandatory step. Since models like **SVM** and **K-Means** rely on **Distances**, scaling prevents features with large values from dominating the model's calculations.
* **Clustering Insights:** While clustering helped in exploring the data structure, the discovered clusters (K-Means & Hierarchical) did not align perfectly with the true labels, making them less suitable for direct classification in these cases.

## 4. Technologies Used
* **Language:** Python
* **Environment:** Google Colab
* **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn.

## 5. Project Files
For the detailed analysis, ROC curves, and confusion matrices:
* **Part 1: Classification (Naive Bayes & Logistic Regression)**
  * [View Source Code (Colab))](./ML1part1_)
  * [View Source Code (Colab)](./ML1part2_)
  * [View Full Technical Report (PDF)](./ML1.pdf)

* **Part 2: SVM & Clustering (K-Means, Hierarchical)**
  * [View Source Code (Colab)](./ML2.ipynb)
  * [View Full Technical Report (PDF)](./ML2.pdf)
