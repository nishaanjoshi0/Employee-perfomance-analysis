# **Employee Performance Prediction Model**

### **Project Overview**
This data science project aims to predict employee performance ratings based on various factors within the dataset, supporting hiring decisions and guiding strategies to enhance overall performance across departments.

### **Goals and Objectives**
- **Department-wise Performance Analysis:** Identify department-specific performance patterns.
- **Key Performance Drivers:** Determine the top factors impacting employee performance.
- **Predictive Model:** Develop a trained machine learning model to predict performance ratings for future hires.
- **Performance Improvement Recommendations:** Provide insights and recommendations based on the analysis to help improve employee performance.

### **Dataset**
- **Size:** 1,200 rows, 28 columns.
- **Structure:** Features are a mix of 19 quantitative (11 numeric, 8 ordinal) and 8 qualitative variables. The target variable (Performance Rating) is ordinal, making this a classification problem.
- **Notable Features:** Important features identified include environmental satisfaction, salary hike percentage, and tenure in current role.

### **Methodology**

1. **Exploratory Data Analysis (EDA):**
   - Conducted univariate, bivariate, and multivariate analyses to uncover patterns and relationships.
   - Analyzed correlation to discover key performance-related features like **EmpEnvironmentSatisfaction**, **EmpLastSalaryHikePercent**, and **EmpWorkLifeBalance**.
   - Used various plots (e.g., histograms, bar plots, violin plots) for visualization.

2. **Data Preprocessing:**
   - **Encoding:** Applied frequency and manual encoding for categorical data.
   - **Outlier Handling:** Used IQR to address outliers in non-normally distributed features.
   - **Feature Transformation:** Applied square root transformations for skewed features to improve model input.
   - **Scaling:** Standardized data to prepare for modeling.
   - **Dimensionality Reduction:** Performed PCA, retaining 25 principal components to maximize information with minimal variance loss.

3. **Modeling:**
   - Selected models: Support Vector Classifier, Random Forest Classifier, and Multilayer Perceptron (MLP) neural network.
   - Achieved best accuracy (95.8%) with MLP, which was selected for final predictions.
   - Addressed data imbalance with **SMOTE** (Synthetic Minority Oversampling Technique) before training.

4. **Feature Importance Analysis:**
   - Identified top factors affecting performance ratings, including environment satisfaction, salary hike, and experience in the current role.

5. **Recommendations:**
   - Focus on improving employee satisfaction in workplace environment, work-life balance, and regular salary hikes.
   - Target recruitment in departments like HR where females tend to outperform, and consider tenure in role for identifying high performers.

### **Tools & Libraries Used**
- **Tools:** Jupyter Notebook
- **Libraries:** Pandas, Numpy, Matplotlib, Seaborn, Scipy, Sklearn, Pickle.

### **Conclusion**
The project successfully provided a predictive model and actionable insights that can support data-driven hiring and management decisions. Improving employee satisfaction and tailoring hiring practices based on performance trends can significantly enhance organizational productivity and employee retention.
