# <p align=center> Capstone Project 24.1: Final Report

## Quick links
* Link to the dataset used in this analysis can be found <a href="https://github.com/Cxpher/bcc/blob/main/data/data.csv">here</a>.
* Link to Jupiter Notebook containing code and visualization for the performed analysis can be found <a href="https://github.com/Cxpher/bcc/blob/main/main_notebook.ipynb">here</a>.
* Link to folder containing all saved visualized plots depicted in the Jupiter Notebook can be found <a href="https://github.com/Cxpher/bcc/tree/main/data/images">here</a>.

## Context
Breast cancer affects many women in today's modern society. Based on research performed by International Agency for Research on Cancer (IARC), the study finds that on average, 1 in 20 women worldwide will be diagnosed with breast cancer in their lifetime, and that if current rates continue, by 2050 there will be 3.2 million new breast cancer cases and 1.1 million breast cancer-related deaths per year. As such, early detection helps and machine learning can help doctors verify the accuracy of their initial diagnosis. 

## Business goal
However, minimizing false negatives is important even if we predict false positives. This prevents unnecessary grief and apply treatment and dispending medication incorrectly. My goal is to understand what factors are indicative of breast cancer and make best cancer predictions with a test dataset or potentially new generalized samples so that doctors can use this model to make accurate predictions.

<br/><br/>
**Determining what features are indicative of a malignant tumor growth in the breast would allow doctors to confidently apply treatment early.**

## Model selection justification
1. Logistic regression
   Simple and efficient model that can map relationships between features and the target variable. It gives you a probability.

2. K-Nearest Neighbors
   Simple model that can be used to do classification. It's good for small datasets like the one used here and does not require much knowledge of the data in terms of samples.

3. Random Forests
   It builds multiple forests and merges their predictions (ensemble) for making a more accurate prediction. It does not overfit easily and even if the features are non-linear, it handles those relationships well.

4. Support Vector Machines
   Very good at finding optimal decision boundaries and not prone to overfitting. Can handle both linear and non-linear relationships between features well using kernal functions. Handles outliers in the data very well.

## Table of findings - Concluding hypothesis

|No. | Findings | Remarks |
|:--- |:---	  |:---      |
|1.  | Discovered high positive correlation between a positive diagnosis and various features of the tumor. |      |		
|2.  | These features include concave area_worst, concave points_worst, perimeter_worst, radius_worst + concave points_mean and perimeter_mean. |      |
|3.  | Logistic regression model is the most accurate in prediction. |      |
|4.  | Support Vector Machines model is a close 2nd. |      |
|5.  | The condition of the car matters the most. Only cars that are in 'like new', 'excellent' or 'good condition' hold any value. |      |
|6.  | Cars that are dated in the last 5 or so years hold the most value. Anything older drops price significantly. |      |
|7.  | Only cars with clean title status have reasonable value. |      |
|8.  | White color cars seems to be the most popular. |      |

