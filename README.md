# Exploratory Data Analysis #

Data Source: https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/haberman.csv

The dataset contains a study conducted between 1958 and 1970 at the University of Chicago on survival of patients who had undergone surgery for breast cancer.

## Attribute Information: ##

    Age of patient
    Patient’s year of operation
    Number of positive lymph nodes detected
    Survival Status (1 = survived 5 years; 2 = died within 5 year)

## Objective ##

To analyze the data to know, how to predict a patient will survive or not, based on his age, number of positive lymph nodes and year in which the operation was conducted.

## Multi-variate Analysis ##


![Pair Plots](https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/4.2PairPlots.png)

## &nbsp; 2D Scatter Plot &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 2D Scatter Plot with Color Coding ##

![2D Scatter Plot](https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/4.1.1ScatterPlot.png) ![2D Scatter Plot with Legend](https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/4.1.2ScatterPlotColorCoding.png)

## Univariate Analysis ##

### CDF ###

![CDF PDF](https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/3.2CDF.png)

### Box Plot ###

![Box Plot](https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/3.3BoxPlot.png)

### Violin Plot ###

![Violin Plot](https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/3.4ViolinPlot.png)

### &nbsp; &nbsp; &nbsp; &nbsp; Age PDF &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Year PDF &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Nodes PDF ###

<img src="https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/3.1.1AgePDF.png" width="285"> <img src="https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/3.1.2YearPDF.png" width="285"> <img src="https://github.com/AdroitAnandAI/Exploratory_Data_Analysis-EDA/blob/master/Images/3.1.3NodesPDF.png" width="290">

## Conclusion ##

### High-Level Analysis ###
1. Haberman is an imbalanced dataset with 224 survived patients & 81 otherwise
2. To make haberman balanced, either under-sample positive class or over-sample negative class. In imbalanced sets, classification algorithms like KNN will favour majority class.
3. 25% of patients dont have any positive lymph node, 50% patients have <=1 and 75% have <= 4 positive lymph nodes. Maximum number of lymph nodes = 52 seems very rare.
4. 50% of patients are in 44-61 age group, though age ranges from 30 to 83.
5. Haberman doesnt have missing values, hence data imputation is not required.

### Univariate Analysis ###
1. PDF: The number of positive lymph nodes are highly dense between 0-5
2. CDF: Nearly 80% of positive lymph nodes are less than 5
3. Box-Plot: Patients who were treated in later years had higher chances of survival.
4. Box-Plot: Patients with higher # of positive lymph nodes has much less chances of survival.
5. Violin-Plot: Same conclusions as in Box Plot.

### Multi-variate Analysis & Conclusion ###
1. With given features, survived & non-survived patient data points show overlapping behaviour. It is difficult to predict survivability with good accuracy as the data is not clearly separable.
2. Among the pair plots, ’Year of Operation vs Lymph Nodes’ plot provides better seperation.
3. ’Age vs Lymph’ Nodes plot could also be used for classification.





