# Decision Tree Classifier on Iris Dataset

## Project Overview

This project implements a Decision Tree Classifier using Python and the scikit-learn library to solve a classic multi-class classification problem: classifying Iris flower species. The primary goal is to accurately predict the species (Setosa, Versicolor, or Virginica) based on four key physical features.

### Key Highlights

* **Dataset:** Iris Dataset (a benchmark in machine learning).
* **Model:** Scikit-learn's `DecisionTreeClassifier`.
* **Performance:** Achieved a robust test set **Accuracy of 95.56% (approx. 96%)**.
* **Interpretability:** The project includes a visualization of the trained decision tree, making the model's decision-making process completely transparent.

## Dataset Details

The Iris dataset contains 150 instances of Iris flowers, with 50 instances for each of the three species, making it a perfectly balanced dataset.

| Feature | Description |
| :--- | :--- |
| **sepal_length** | Length of the sepal in centimeters. |
| **sepal_width** | Width of the sepal in centimeters. |
| **petal_length** | Length of the petal in centimeters. |
| **petal_width** | Width of the petal in centimeters. |
| **species (Target)** | Iris Setosa, Iris Versicolor, or Iris Virginica. |

## Methodology

The classification pipeline followed industry-standard steps:

1.  **Data Loading and EDA:** The dataset was loaded, converted into a Pandas DataFrame, and inspected for missing values (none found) and class balance (perfectly balanced). Exploratory visualizations (e.g., box plots and pair plots) were used to understand the separability of classes.
2.  **Data Preparation:** Features (X) and the target (y) were separated. A standard **80/20 Train-Test Split** was applied with a fixed random state for reproducibility.
3.  **Model Training:** A Decision Tree Classifier was instantiated and trained on the 80% training subset.
4.  **Model Evaluation:** The model's performance was rigorously evaluated on the 20% held-out test set using:
    * Overall Accuracy
    * Classification Report (Precision, Recall, F1-Score)
    * Confusion Matrix
5.  **Model Visualization:** The final decision rules were plotted using `sklearn.tree.plot_tree`.

## Results

The model achieved high accuracy, successfully distinguishing all Setosa samples and making only minor errors between the more similar Versicolor and Virginica classes.

**Overall Test Accuracy: 95.56%**

| Class (Species) | Precision | Recall | F1-Score | Support |
| :--- | :--- | :--- | :--- | :--- |
| **Iris Setosa** | 1.00 | 1.00 | 1.00 | 18 |
| **Iris Versicolor**| 0.82 | 1.00 | 0.90 | 9 |
| **Iris Virginica**| 1.00 | 0.89 | 0.94 | 18 |

### Decision Tree Visualization

This visualization is the core component of the project, clearly showing the splitting nodes based on features like Petal Length and Petal Width.

## Getting Started

### Prerequisites

To run this project locally, you need a Python environment with the following packages:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

### File Structure

The project is contained within a single notebook file.

Desition_Tree_Iris_Dataset
```
├── Desicion_Tree_Iris_Dataset.ipynb  
├── README.md
```

### Running the Project

1. Clone this repository:
```bash
git clone https://github.com/PranayDomal/Desition_Tree_Iris_Datadet.git
```
2. Navigate to the project directory.
3. Open and run the Jupyter Notebook:
```bash
jupyter notebook Desicion_Tree_Iris_Dataset.ipynb
```
### Author
https://www.linkedin.com/in/pranay-domal-a641bb368/
