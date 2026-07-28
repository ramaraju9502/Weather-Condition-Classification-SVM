# Weather Condition Classification using Support Vector Machine (SVM) and Open-Meteo API

## Objective

The objective of this project is to develop a Support Vector Machine (SVM) classification model to classify weather conditions as **Warm** or **Cool** based on meteorological observations obtained from the Open-Meteo Weather API. The project demonstrates the complete machine learning workflow, including data collection from an API, preprocessing, feature scaling, model development, prediction, and performance evaluation using standard classification metrics.

---

## API Documentation Link

**Open-Meteo Weather API**

Documentation: https://open-meteo.com/

---

## Libraries Used

The following Python libraries were used in this project:

- Pandas
- NumPy
- Requests
- Matplotlib
- Seaborn
- Scikit-learn

Modules from Scikit-learn:

- SVC
- StandardScaler
- train_test_split
- accuracy_score
- precision_score
- recall_score
- f1_score
- confusion_matrix
- ConfusionMatrixDisplay

---

## Methodology

The project was completed using the following steps:

1. Collected weather data from the Open-Meteo Weather API.
2. Converted the JSON response into a Pandas DataFrame.
3. Created a target variable (**Weather_Class**) based on temperature values.
4. Checked for missing values and removed unnecessary columns if required.
5. Encoded the target variable into numerical values.
6. Standardized the feature values using **StandardScaler**.
7. Split the dataset into training (80%) and testing (20%) sets.
8. Built an **SVM Classifier** using the **RBF kernel**.
9. Predicted weather classes for the testing dataset.
10. Evaluated the model using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix.

---

## Results

The Support Vector Machine classifier successfully classified weather conditions into **Warm** and **Cool** categories using meteorological features obtained from the Open-Meteo API.

Performance was evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score

A Confusion Matrix was generated to visualize the classification performance. The evaluation results demonstrated that feature scaling significantly improved the effectiveness of the SVM classifier by ensuring balanced distance calculations between feature values.

---

## Conclusion

This project demonstrates the effectiveness of Support Vector Machines (SVM) for weather condition classification using real-time meteorological data from the Open-Meteo API. After preprocessing the data and applying feature scaling, the SVM model accurately classified weather conditions into Warm and Cool categories. Feature scaling played an important role in improving model performance because SVM relies on distance-based optimization. One major advantage of SVM is its ability to perform well on high-dimensional datasets while maintaining good generalization. However, a limitation of SVM is that it can be computationally expensive for large datasets and requires careful parameter selection. Overall, the model provides an efficient and reliable approach for weather classification tasks.
