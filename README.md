# Experiment Overview

## Project Title: Predicting Student GPA Using Linear Regression

### Description
This project explores the factors influencing student academic performance, specifically Grade Point Average (GPA), using a linear regression model. The experiment aims to identify the impact of various factors on GPA.

### Dataset
The dataset consists of **2,392 student records** with **15 features**, including:
- **StudyTimeWeekly**: Hours dedicated to studying per week
- **Absences**: Number of classes missed
- **Tutoring**: Binary indicator for tutoring support
- **Extracurricular**: Participation in extracurricular activities
- **ParentalSupport**: Level of parental involvement
- **ParentalEducation**: Educational background of parents
- **GPA**: Target variable (continuous, ranging from 0.0 to 4.0)

The dataset has a **usability index of 10** on Kaggle, with no missing values, ensuring minimal preprocessing requirements.

### Methodology
- **Exploratory Data Analysis (EDA)**: Conducted correlation analysis and visualizations to understand feature relationships.
- **Feature Selection**: Selected key features based on Pearson correlation and domain knowledge.
- **Model Implementation**: Used `scikit-learn` to implement a linear regression model.
- **Cross-Validation**: Applied **5-fold cross-validation** to ensure robustness.
- **Performance Evaluation**:
    - **Mean Squared Error (MSE)**: 0.0506
    - **R² Score**: 0.9387 (indicating strong predictive performance)

### Key Findings
- **Absences (-0.92 correlation with GPA)** had the most significant negative impact.
- **StudyTimeWeekly (0.18) and ParentalSupport (0.19)** showed weak positive correlations.
- **Tutoring and Extracurricular Activities** moderately influenced GPA.
- The linear regression model successfully captured academic performance trends with high accuracy.

### Repository Contents
- `student_pred.ipynb`: Jupyter notebooks for data analysis and model implementation
- `Student_performance_data_.csv`: Dataset files used for training and evaluation
- `README.md`: Project documentation

### References
- [IBM: What is Linear Regression?](https://www.ibm.com/think/topics/linear-regression)
- [Analytics Vidhya: Linear Regression Guide](https://www.analyticsvidhya.com/blog/2021/10/everything-you-need-to-know-about-linear-regression/)
- [Scikit-learn: Cross-validation](https://scikit-learn.org/stable/modules/cross_validation.html)
- [Pure Storage: Machine Learning Performance Metrics](https://www.purestorage.com/knowledge/machine-learning-performance-metrics.html)

### How to Use
1. Clone the repository:
    ```bash
    git clone https://github.com/mrchreesa/linear-regression.git
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook for data exploration and model training.

### Future Work
- Explore **non-linear models** (decision trees, neural networks) for potential accuracy improvements.
- Incorporate **additional student attributes**, such as socioeconomic factors and motivation levels.
- Develop a **real-time prediction API** for educational institutions.

This repository serves as a comprehensive resource for understanding and predicting student academic performance using machine learning techniques.
