# Mental Fatigue Analysis and Lifestyle Impact

## Project Overview
This project investigates the factors associated with **mental fatigue** using lifestyle and occupational data. The dataset contains **15,000 observations** describing individuals’ stress levels, screen time, sleep behaviour, physical activity, and occupation.

The objective of the project is to:

- Identify key factors associated with **mental fatigue**
- Analyse differences in fatigue levels across **occupations**
- Examine the relationship between **lifestyle behaviours and fatigue**
- Use **machine learning models** to predict mental fatigue
- Simulate how improvements in lifestyle may reduce fatigue levels

Both **statistical analysis and machine learning techniques** were applied to better understand the drivers of mental fatigue.

---

## Dataset
The dataset includes **15,000 observations** with features describing lifestyle habits, work characteristics, and health indicators.

Key variables include:

- Stress Level  
- Daily Screen Time (hours)  
- Sleep Duration  
- Sleep Quality Score  
- Exercise Duration (minutes)  
- Physical Activity Level  
- Occupation  
- Mental Fatigue Score (target variable)

These features were used to analyse behavioural patterns and evaluate how lifestyle factors influence mental fatigue.

---

## Methodology

### 1. Data Cleaning and Preprocessing
The dataset was prepared using Python by:

- Checking for **missing values**
- Removing **duplicate observations**
- Selecting relevant lifestyle variables for modelling
- Preparing features for regression and machine learning analysis

**Libraries used:**

- Pandas  
- NumPy  
- Scikit-learn  
- Statsmodels  
- Seaborn / Matplotlib  

---

### 2. Exploratory Data Analysis
Exploratory analysis was conducted to understand relationships between variables.

Key analyses included:

- Correlation analysis between lifestyle variables and mental fatigue
- Visualization of relationships between stress, screen time, sleep quality, and fatigue
- Comparison of mental fatigue across different occupations

The analysis revealed that **stress level has the strongest relationship with mental fatigue**, while screen time and sleep behaviour show smaller but meaningful associations.

---

### 3. Statistical Analysis
Multiple statistical techniques were applied to validate observed relationships.

**Multiple Linear Regression**

Regression analysis was used to examine how lifestyle factors influence mental fatigue. Results indicated:

- **Stress level is the strongest predictor of mental fatigue**
- Screen time has a smaller but statistically significant relationship
- The regression model explained approximately **90% of the variance in mental fatigue (R² ≈ 0.90)**

**Occupational Analysis**

Mental fatigue levels were compared across occupations. Students exhibited the **highest average mental fatigue**, although most occupational differences were relatively small.

**ANOVA and Post-hoc Tests**

A one-way ANOVA was conducted to test whether fatigue levels differ across occupations. The results indicated **statistically significant differences between some occupational groups**. Post-hoc Tukey tests showed that **students exhibited significantly higher fatigue compared to designers**, while most other occupational differences were not statistically significant.

---

## Model Comparison

Several regression-based machine learning models were tested to predict mental fatigue:

- **Linear Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

Model performance comparison:

| Model | R² | MAE |
|------|------|------|
| Gradient Boosting | 0.9028 | 0.6646 |
| Linear Regression | 0.9026 | 0.6567 |
| Random Forest | 0.8962 | 0.6866 |

All models achieved **similar performance (R² ≈ 0.90)**, suggesting that the relationship between lifestyle factors and mental fatigue is largely **linear**.

Linear Regression achieved the **lowest prediction error**, indicating that a simple interpretable model performs as well as more complex algorithms.

---

## Lifestyle Simulation

A scenario simulation was performed using the trained model to estimate how mental fatigue may change under improved lifestyle conditions.

Two scenarios were compared:

**Current lifestyle**
- High stress level  
- Long screen time  
- Poor sleep quality  
- Limited exercise  

**Improved lifestyle**
- Lower stress level  
- Reduced screen time  
- Higher sleep quality  
- Increased exercise duration  

Model predictions suggest that **improving lifestyle behaviours may substantially reduce predicted mental fatigue levels**, particularly through reductions in stress and improvements in sleep quality.

---

## Key Findings

The analysis produced several important insights:

- **Stress level is the strongest predictor of mental fatigue**
- Screen time has a smaller but statistically significant association with fatigue
- Students show the **highest average mental fatigue levels**
- Most occupational differences in fatigue are relatively small
- Machine learning models confirm the importance of **stress and sleep quality** in predicting fatigue

Overall, the findings highlight the importance of **lifestyle management, stress reduction, and sleep quality** in improving mental well-being.
