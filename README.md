# housing_price_regression
To build a predictive model that estimates the market value of a house based on its physical attributes and geographical location
📌 Project OverviewThis project implements a Multiple Linear Regression model to predict the median value of owner-occupied homes in Boston. By analyzing 13 distinct features—ranging from crime rates to property tax levels—the model identifies key drivers of real estate pricing.

📊 Dataset DescriptionThe dataset contains 506 observations and 14 variables. The target variable is medv (Median value of owner-occupied homes).

#Column                               # Description
crim                                  Per capita crime rate by town
zn                                    Proportion of residential land zoned for large lots
indus                                 Proportion of non-retail business acres per town
chas                                  Charles River dummy variable (1 if tract bounds river; 0 otherwise)
nox                                   Nitric oxides concentration (parts per 10 million)
rm                                    Average number of rooms per dwelling
age                                   Proportion of owner-occupied units built prior to 1940
dis                                   Weighted distances to five Boston employment centres
rad                                   Index of accessibility to radial highways
tax                                   Full-value property-tax rate per $10,000
ptratio                               Pupil-teacher ratio by town
b                                     Proportion of residents of African American descent
lstat%                                lower status of the population
medv (Target)                         Median value of owner-occupied homes in $1000s

**⚙️ Technical Implementation1. **
1.Exploratory Data Analysis (EDA)
      **Correlation Analysis:** Identified that rm (rooms) has a strong positive correlation with price, while lstat (lower status population) has a strong negative correlation.
      **Feature Scaling:** Applied standardization to handle the varying scales of columns like tax (hundreds) vs nox (decimals)
      
2. Model Performance:
          **R^2 Score:** Evaluates how much of the price variance is explained by the features.
          **Mean Squared Error (MSE):** Measures the average squared difference between estimated and actual values.


**🛠️ Installation & Usage**

   Clone the repository:Bashgit clone https://github.com/your-username/boston-housing-regression.git
   Install requirements:Bashpip install pandas scikit-learn matplotlib seaborn
   Run the prediction script:Bashpython boston_model.py
