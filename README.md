# Heart Attack Analysis And Prediction
## Project Content

#### Introduction
1.1 Examining the Project Topic

1.2 Recognizing Variables In Dataset

#### First Organization
2.1 Required Python Libraries

2.1.1 Basic Libraries

2.2 Loading the Dataset

2.3 Initial analysis on the dataset

2.3.1 Analysis Outputs(1)

#### Preparation for Exploratory Data Analysis(EDA)

3.1 Examining Missing Values

3.2 Examining Unique Values

3.2.1 Analysis Outputs(2)

3.3 Separating variables (Numeric or Categorical)

3.4 Examining Statistics of Variables

3.4.1 Analysis Outputs(3)

#### Exploratory Data Analysis(EDA)

4.1 Uni-variate Analysis

4.1.1 Numerical Variables(Analysis with Distplot)

4.1.1.1 Analysis Outputs(4)

4.1.2 Categorical Variables(Analysis with Pie Chart)

4.1.2.1 Analysis Outputs(5)

4.1.2.2 Examining the Missing Data According to the Analysis Result

4.2 Bi-Variate Analysis

4.2.1 Numerical Variables - Target Variable(Analysis with FacetGrid)

4.2.1.1 Analysis Outputs(6)

4.2.2 Categorical Variables-Target Variable(Analysis with Count Plot)

4.2.2.1 Analysis Outputs(7)

4.2.3 Examining Numeric Variables Among Themselves(Analysis with Pair Plot)

4.2.3.1 Analysis Outputs(8)

4.2.4 Feature Scaling with the RobustScaler Method

4.2.5 Creating a New DataFrame with the Melt() Function

4.2.6 Numerical - Categorical Variables (Analysis with Swarm Plot)

4.2.6.1 Analysis Outputs(9)

4.2.7 Numerical - Categorical Variables (Analysis with Box Plot)

4.2.7.1 Analysis Outputs(10)

4.2.8 Relationships between variables(Analysis with Heatmap)

4.2.8.1 Analysis Outputs(11)

#### Preparation for Modelling

5.1 Dropping Columns with Low Correlation

5.2 Struggling Outliers

5.2.1 Visualizing outliers

5.2.1.1 Analysis Outputs(12)

5.2.2 Dealing with outliers

5.2.2.1 Trtbps Variable

5.2.2.2 Thalach Variable

5.2.2.3 Oldpeak Variable

5.3 Determining Distributions of Numeric Variables

5.4 Transformation Operations on Unsymmetrical Data

5.5 Applying One Hot Encoding Method to Categorical Variables

5.6 Feature Scaling with the RobustScaler Method for Machine Learning Algorithms

5.7 Separating Data into Test and Training Set

#### Modelling

6.1 Logistic Regression Algorithm

6.1.1 Cross Validation

6.1.2 Roc Curve and Area Under Curve(AUC)

6.1.3 Hyperparameter Optimization(With GridSearchCV)

6.2 Decision Tree Algorithm

6.3 Support Vector Machine Algorithm

6.4 Random Forest Algorithm

6.4.1 Hyperparameter Optimization(With GridSearchCV)

#### Project Conclusion
## 1. Introduction

1.1 Examining the Project Topic 

What is a Heart Attack?


The medical name of heart attack is “Myocardial infarction”.
Heart attack in short; It is the occlusion of the vessel by plaque-like lesions filled with cholesterol and fat.
The lesion is called abnormal conditions that occur in the organs where the disease is located.
As a result of the blockage, the blood flow is completely cut off and a heart attack that can lead to death occurs.
How does a Heart Attack occure?


The heart is a powerful pump that pumps blood throughout the body 60-80 times per minute at rest.
While meeting the blood needs of the whole body, it also needs to be fed and taken blood.
These vessels that feed the heart itself are called coronary arteries.
Coronary insufficiency occurs when there is a disruption in the circulation of the coronary arteries.
The cases of coronary insufficiency vary according to the type, degree and location of the stenosis in the coronary vessels.
While some patients may have chest pain that occurs only during physical activity and is relieved by rest, sometimes a heart attack may occur as a result of sudden occlusion of the vessels, starting with severe chest pain and leading to sudden death.
What are the symptoms of a Heart Attack?


1.2 Recognizing Variables in Dataset

Variable definitions in the Dataset

Age: Age of the patient
Sex: Sex of the patient
exang: exercise induced angina (1 = yes; 0 = no)
ca: number of major vessels (0-3)
cp: Chest Pain type chest pain type
Value 1: typical angina
Value 2: atypical angina
Value 3: non-anginal pain
Value 4: asymptomatic
trtbps: resting blood pressure (in mm Hg)
chol: cholestoral in mg/dl fetched via BMI sensor
fbs: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
_restecg: resting electrocardiographic results
Value 0: normal
Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
thalach: maximum heart rate achieved
target: 0= less chance of heart attack 1= more chance of heart attack
Additional variable descriptions to help us

age - age in years

sex - sex (1 = male; 0 = female)

cp - chest pain type (1 = typical angina; 2 = atypical angina; 3 = non-anginal pain; 0 = asymptomatic)

trestbps - resting blood pressure (in mm Hg on admission to the hospital)

chol - serum cholestoral in mg/dl

fbs - fasting blood sugar > 120 mg/dl (1 = true; 0 = false)

restecg - resting electrocardiographic results (1 = normal; 2 = having ST-T wave abnormality; 0 = hypertrophy)

thalach - maximum heart rate achieved

exang - exercise induced angina (1 = yes; 0 = no)

oldpeak - ST depression induced by exercise relative to rest

slope - the slope of the peak exercise ST segment (2 = upsloping; 1 = flat; 0 = downsloping)

ca - number of major vessels (0-3) colored by flourosopy

thal - 2 = normal; 1 = fixed defect; 3 = reversable defect

num - the predicted attribute - diagnosis of heart disease (angiographic disease status) (Value 0 = < diameter narrowing; Value 1 = > 50% diameter narrowing)


# Project Conclusion

The activities we carried out within the scope of the project are as follows:

Within the scope of the project, we first made the data set ready for Exploratory Data Analysis(EDA)

We performed Exploratory Data Analysis(EDA).

We analyzed numerical and categorical variables within the scope of univariate analysis by using Distplot and Pie Chart graphics.

Within the scope of bivariate analysis, we analyzed the variables among each other using FacetGrid, Count Plot, Pair Plot, Swarm plot, Box plot, and Heatmap graphics.

We made the data set ready for the model. In this context, we struggled with missing and outlier values.

We used four different algorithms in the model phase.

We got 87% accuracy and 88% AUC with the Logistic Regression model.

We got 75% accuracy and 75% AUC with the Decision Tree Model.

We got 83% accuracy and 90% AUC with the Support Vector Classifier Model.

And we got 83.8% accuracy and 93% AUC with the Random Forest Classifier Model.

When all these model outputs are evaluated, we prefer the model we created with the **Random Forest Algorithm**, which gives the best results.