# Data Analytics Iris Research
** by Serhii Spitsyn**

## Intro
Data analysis is a critical part of modern scientific research and business intelligence, as it allows large amounts of information to be understood and interpreted. One of the most well-known datasets for newcomers to the field is the [Iris database](https://en.wikipedia.org/wiki/Iris_flower_data_set), which is often used as an introduction to statistical analysis. 
Let's look at the key aspects of data analysis using the Iris database as an example and highlight the main typical problems that analysts may face whose research and conclusions were taken from selected freely available sources.

## About the data
This is one of the earliest datasets used in the literature on classification methods and widely used in statistics and machine learning.  The data set contains 3 classes of 50 instances each, where each class refers to a type of iris plant.  One class is linearly separable from the other 2; the latter are not linearly separable from each other. This data was collected by [Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher) in 1936.

### Data Reference
[Link for Iris data site](https://archive.ics.uci.edu/dataset/53/iris)

### Description
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

# Data Analysis

## Using the Iris Database in Data Analysis

### Classification
The Iris database is often used for classification tasks where the goal is to determine the iris species based on petal and sepal measurements. This is a typical example of a supervised learning problem, where machine learning algorithms such as logistic regression, decision trees, or neural networks are trained on well-defined data and then predict the shape of the iris.

### Clustering
Another popular method of analysis is clustering, which allows you to group data based on the similarity of their characteristics without first defining class labels. Algorithms, such as K-means, can be used to determine internal structures in an Iris dataset.

## Problems in analyzing Iris database data
### Dataset size
One of the main problems with the Iris database is its small size. In a world dominated by big data, models trained on such small datasets may not adequately reflect the complexity of real-world tasks and transfer learned patterns to new, larger data.
The Iris dataset consists of a total of 150 records divided into three classes. This number may be sufficient to demonstrate the functionality of statistical methods or machine learning algorithms at a basic level, but it does not provide sufficient variability and data volume to model complex [Exploratory Data Analysis on Iris Dataset](https://www.geeksforgeeks.org/exploratory-data-analysis-on-iris-dataset/) tasks.

### Class imbalance
An equal distribution between classes helps to avoid model bias. The solution to this problem is to check the distribution of classes and adjust the balance of the data as needed [Categorical Exploratory Data Analysis: From Multiclass Classification and Response Manifold Analytics Perspectives of Baseball Pitching Dynamics](https://www.mdpi.com/1099-4300/23/7/792).
Although classes are relatively evenly represented in the Iris database, in real-world problems, researchers often encounter class imbalances, where some classes have significantly more or fewer samples. Such imbalances can affect the accuracy of classification models.

### Simplified features
Irises in the database are described by only four characteristics, which is a very simplified representation. Real-world systems often require more factors and relationships to be taken into account [Investigating the Iris dataset](https://www.angela1c.com/projects/iris_project/investigating-the-iris-dataset/). 
Using only four characteristics to describe iris flowers significantly limits the model's ability to analyze and understand the biological characteristics of the species in detail. This simplification can lead to incomplete or incorrect interpretation of the data, especially in complex biological or environmental studies.
In real-world biological and ecological systems, flowers and plants interact with the environment and other organisms through many more factors than just the size of their parts. Ignoring such factors can make it difficult to use this dataset for deeper or more general scientific research.


### No Noise and No Emissions
Outlier handling: Outliers can degrade analysis results, so identifying and removing them is critical. Outliers are identified using visual techniques and filtered from the data to ensure the accuracy of the analysis [Exploratory Data Analysis : Iris Dataset](https://medium.com/analytics-vidhya/exploratory-data-analysis-iris-dataset-4df6f045cda).
The data in the Iris database is well-prepared and contains a minimum of noise and emissions. In practice, data is often noisy and contains errors or anomalies, making it much more difficult to analyze.

## Conclusion
The Iris database remains a popular choice for introduction to machine learning and statistics, but it's important to understand its limitations. When analyzing, care must be taken when applying the conclusions drawn from this dataset to more complex or diverse data to avoid errors and misunderstandings in their models. 
In conclusion, it is necessary to underestimate the preliminary analysis of the data to determine the relevance of the data and an objective assessment of the results obtained after analysis, or visualization of the data.

## Analysis of research methods

### Overview of methodologies
Exploratory data analysis of the Iris suite demonstrates the basic data processing and visualization techniques used to identify structures and distributions in data. Different approaches to analysis from the Iris dataset, as described in the articles [Exploratory Data Analysis on Iris Dataset](https://www.geeksforgeeks.org/exploratory-data-analysis-on-iris-dataset/) and [Exploratory Data Analysis : Iris Dataset](https://medium.com/analytics-vidhya/exploratory-data-analysis-iris-dataset-4df6f045cda), highlight it`s usefulness in improving data understanding and data modeling.

### Data preprocessing
Processing of duplicates and missing values is performed using the isnull() and drop_duplicates() methods of the pandas library, which allows you to maintain high data quality [Exploratory Data Analysis of Iris Dataset](https://medium.com/@nirajan.acharya666/exploratory-data-analysis-of-iris-dataset-9c0df76771df).

### Totals
The describe() function is used to get quick statistical summaries, which is an integral part of preparing for a more detailed analysis [Exploratory Data Analysis of IRIS Data Set Using Python](https://medium.com/@avulurivenkatasaireddy/exploratory-data-analysis-of-iris-data-set-using-python-823e54110d2d).

### Visualization techniques
Visual generalization of data distributions and potential outliers is provided using histograms, box plots, cello charts, as well as pair plots and heatmaps [Python For Data Science – Exploratory Data Analysis – IRIS Dataset](https://notepub.io/notes/programming-languages/python-for-data-science/python-for-data-science-exploratory-data-analysis-iris-dataset/).

# Data Processing by Software 

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

## Layout Plot

### Distribution of 
!["Distribution of "](https://github.com/ShamansIT)

## Goals
- To accurately segment iris into distinct clusters
- To develop skills in data preprocessing, feature selection, and the application of unsupervised learning techniques
- To establish a versatile clustering pipeline applicable to subsequent projects

## References

[Exploratory Data Analysis on Iris Dataset](https://www.geeksforgeeks.org/exploratory-data-analysis-on-iris-dataset/)

[Exploratory Data Analysis : Iris Dataset](https://medium.com/analytics-vidhya/exploratory-data-analysis-iris-dataset-4df6f045cda)

[Exploratory Data Analysis of Iris Dataset](https://medium.com/@nirajan.acharya666/exploratory-data-analysis-of-iris-dataset-9c0df76771df)

[Python For Data Science – Exploratory Data Analysis – IRIS Dataset](https://notepub.io/notes/programming-languages/python-for-data-science/python-for-data-science-exploratory-data-analysis-iris-dataset/)

[Investigating the Iris dataset](https://www.angela1c.com/projects/iris_project/investigating-the-iris-dataset/)

[Categorical Exploratory Data Analysis: From Multiclass Classification and Response Manifold Analytics Perspectives of Baseball Pitching Dynamics](https://www.mdpi.com/1099-4300/23/7/792)

[Analysis of the famous Iris Flower dataset](https://wnellie.tumblr.com/post/143155937907/analysis-of-the-famous-iris-flower-dataset-part)

[Exploratory Data Analysis of IRIS Data Set Using Python](https://medium.com/@avulurivenkatasaireddy/exploratory-data-analysis-of-iris-data-set-using-python-823e54110d2d)

[Discriminating Fisher's iris data by using the petal areas](https://blogs.sas.com/content/iml/2012/08/09/discriminating-fishers-iris-data-by-using-the-petal-areas.html)

[Exploratory Data Analysis: Iris Flower Dataset](https://indeepdata.com/blog/exploratory-data-analysis/)