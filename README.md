# Iris and Breast Cancer Wisconsin Dataset Analysis

This project involves the analysis of two popular datasets: the Iris dataset and the Breast Cancer Wisconsin dataset. The goal is to perform exploratory data analysis (EDA), visualize the data, and apply machine learning models to classify the data.

## Datasets

### Iris Dataset
The Iris dataset contains 150 samples of iris flowers, with 4 features each:
- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

The target variable is the species of the iris flower, which can be one of three classes:
- 0: Setosa
- 1: Versicolor
- 2: Virginica

### Breast Cancer Wisconsin Dataset
The Breast Cancer Wisconsin dataset contains 699 samples, with 9 features each. The target variable is the class of the tumor:
- 2: Benign
- 4: Malignant

## Exploratory Data Analysis (EDA)

### Iris Dataset
1. **Scatter Plots**:
   - Sepal length vs. Sepal width
   - Petal length vs. Petal width

2. **Pair Plots**:
   - Pairwise relationships between all features.

3. **Correlation Heatmap**:
   - Visualize the correlation between features.

4. **Count Plot**:
   - Distribution of target classes.

### Breast Cancer Wisconsin Dataset
1. **Count Plot**:
   - Distribution of target classes.

2. **Correlation Heatmap**:
   - Visualize the correlation between features.

3. **Principal Component Analysis (PCA)**:
   - Reduce dimensionality and visualize explained variance.

## Machine Learning Models

### K-Nearest Neighbors (KNN) Classifier
The KNN classifier is applied to both datasets to classify the target variable. The following steps are performed:

1. **Data Splitting**:
   - Split the data into training and testing sets (80% training, 20% testing).

2. **Feature Scaling**:
   - Standardize the features using `StandardScaler`.

3. **Model Training and Evaluation**:
   - Train the KNN model with different values of `k` (from 1 to 10).
   - Evaluate the model using accuracy score.

### Results

#### Iris Dataset
- The best accuracy is achieved with `k=1`, `k=3`, `k=5`, `k=7`, `k=8`, `k=9`, and `k=10`, with an accuracy of 96.67%.

#### Breast Cancer Wisconsin Dataset
- The best accuracy is achieved with `k=3`, `k=5`, `k=6`, `k=7`, `k=8`, `k=9`, and `k=10`, with an accuracy of 97.14%.

## Visualizations

### Confusion Matrix
- A confusion matrix is plotted to visualize the performance of the KNN classifier on the Breast Cancer Wisconsin dataset.

## How to Run the Code

1. **Install Required Libraries**:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn ucimlrepo
