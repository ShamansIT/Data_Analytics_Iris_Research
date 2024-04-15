# Data_Analytics_Iris_Research
** by Serhii Spitsyn**

## Project Descriptions
Explore the Iris dataset in this repository, featuring data analysis, visualizations, and machine learning models for species classification.

## About the data
This is one of the earliest datasets used in the literature on classification methods and widely used in statistics and machine learning.  The data set contains 3 classes of 50 instances each, where each class refers to a type of iris plant.  One class is linearly separable from the other 2; the latter are not linearly separable from each other.

### Reference
[Link for Iris data site](https://archive.ics.uci.edu/dataset/53/iris)

Number of Instances: 150 (50 in each of three classes)
Number of Attributes: 4 numeric, predictive attributes and the class

Attribute Information:
   1. sepal length in cm
   2. sepal width in cm
   3. petal length in cm
   4. petal width in cm
   5. class: 
      -- Iris Setosa
      -- Iris Versicolour
      -- Iris Virginica
      
## Data Dictionary

| Variable Name |   Role    |     Type     | Description                                         | Units | Missing Values |
|---------------|-----------|--------------|-----------------------------------------------------|-------|----------------|
| sepal length  | Feature   | Continuous   | Length of the sepal                                 | cm    | no             |
| sepal width   | Feature   | Continuous   | Width of the sepal                                  | cm    | no             |
| petal length  | Feature   | Continuous   | Length of the petal                                 | cm    | no             |
| petal width   | Feature   | Continuous   | Width of the petal                                  | cm    | no             |
| class         | Target    | Categorical  | Class of iris plant: Iris Setosa, Iris Versicolour, or Iris Virginica |       | no             |

## Stack
- Data - Python, Jupyter Notebook, Pandas, NumPy, SciPy
- Visualization - Matplotlib
- Streamlit - Python, Pandas
- Version Control and CI/CD - GitHub Projects, GitHub Actions

## Imports
Use pandas for the DataFrame data structure. It allows us to investigate CSV files amongst amongst other features.

## Data Modeling
Adjusting the data types in DataFrames is crucial for enhancing memory efficiency, speeding up calculations, and ensuring the data is compatible with various operations and analytical methods. It is essential to customize these data type adjustments based on the specific needs of your analysis, the characteristics of the data in each column, and your broader data processing goals.

The data type of each column in a DataFrame greatly affects what operations can be performed. Changing these data types may be necessary to improve processing efficiency, enable specific functionalities, or align the data more closely with the best-suited analytical techniques.

## Data Sample Table
| Sepal length (cm) | Sepal width (cm) | Petal length (cm) | Petal width (cm) | Class plants   |
|-------------------|------------------|-------------------|------------------|----------------|
| 5.1               | 3.5              | 1.4               | 0.2              | Iris-setosa    |
| 4.9               | 3.0              | 1.4               | 0.2              | Iris-setosa    |
| 4.7               | 3.2              | 1.3               | 0.2              | Iris-setosa    |
| 6.5               | 3.0              | 5.2               | 2.0              | Iris-virginica |
| 6.2               | 3.4              | 5.4               | 2.3              | Iris-virginica |
| 5.9               | 3.0              | 5.1               | 1.8              | Iris-virginica |


### Advantages of Converting to Category Data Type
Memory Efficiency: Using the category data type, which internally maps categories to integers, generally consumes less memory than string types, particularly when there are few unique categories compared to the total data points.

Performance Enhancement: Categorical data speeds up operations like groupby, sorting, and other vectorized functions, compared to string data.

Semantic Clarity: By converting a column to categorical data type, it explicitly indicates that the data can only take on a set number of distinct categories, improving code readability and understanding.

## Missing data
After analysis Itis DataFraim, it was found that the lost data is completely absent in this Network. Further cleaning of the data at this stage is not required and is not logical from the point of view of data processing performance.

## Project Descriptions





## Layout Plot

### Distribution of 
!["Distribution of "](https://github.com/ShamansIT)

## Goals
- To accurately segment iris into distinct clusters
- To develop skills in data preprocessing, feature selection, and the application of unsupervised learning techniques
- To establish a versatile clustering pipeline applicable to subsequent projects

