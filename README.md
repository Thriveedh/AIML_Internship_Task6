# AIML_Internship_Task6
# K-Nearest Neighbors (KNN) Classification with Decision Boundary Visualization

This task demonstrates how to apply the **K-Nearest Neighbors (KNN)** algorithm on a real-world dataset using **scikit-learn**. It includes full **data preprocessing**, **outlier removal**, **normalization**, and **decision boundary visualization** for different values of K.

## Dataset

Each data point represents measurements of an iris flower, classified into one of three species: *Iris-setosa*, *Iris-versicolor*, or *Iris-virginica*.

## Preprocessing Steps

1. **Removed Unnecessary Columns**:  
   The `Id` column was dropped as it is not useful for classification.

2. **Label Encoding**:  
   The categorical target variable `Species` was converted to numeric using `LabelEncoder`.

3. **Outlier Detection and Removal**:  
   Outliers were detected using the **IQR (Interquartile Range)** method and removed to improve model performance.

4. **Normalization**:  
   Feature values were scaled between 0 and 1 using **Min-Max Normalization** to ensure all features contribute equally to distance calculations in KNN.

## What This Task Does

- Loads and cleans the Iris dataset.
- Preprocesses the data (label encoding, outlier removal, normalization).
- Splits the dataset into training and test sets (80/20).
- Trains a **KNN classifier** for different values of `K` (1, 3, 5, 7, 9).
- Evaluates each model using **accuracy**.
- **Visualizes decision boundaries** using two selected features (e.g., SepalLengthCm and PetalLengthCm).

## Visualizations

For each `K`:
- Decision boundaries are plotted using two features.
- Training data is shown with circle markers `o`.
- Test data is shown with triangle markers `^`.
- Background colors represent regions classified by the KNN model.
