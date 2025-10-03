

# CVD Risk Factor Analysis and Prediction

[](https://www.python.org/downloads/)
[](https://scikit-learn.org/stable/)
[](https://powerbi.microsoft.com/)

-----

##  Project Overview

[cite\_start]This project provides an end-to-end analysis of cardiovascular disease (CVD) risk factors using a public health dataset from Bangladesh. [cite: 22, 31] [cite\_start]The primary objective is to identify key biomarkers for CVD, develop a predictive model for risk stratification, and present the analytical findings through interactive dashboards created in Power BI. [cite: 33, 34, 35, 36, 46] [cite\_start]This project replicates the analytical processes that would be conducted in hospital research departments, health tech startups, or public health organizations. [cite: 23, 24, 25, 26, 27]

-----

##  Table of Contents

  - [Dashboards & Visualizations](https://www.google.com/search?q=%23-dashboards--visualizations)
  - [Project Workflow](https://www.google.com/search?q=%23-project-workflow)
  - [Dataset](https://www.google.com/search?q=%23-dataset)
  - [ Technical Stack](https://www.google.com/search?q=%23%EF%B8%8F-technical-stack)
  - [ Installation & Setup](https://www.google.com/search?q=%23%EF%B8%8F-installation--setup)
  - [ How to Run](https://www.google.com/search?q=%23-how-to-run)
  - [ Key Analysis and Results](https://www.google.com/search?q=%23-key-analysis-and-results)
  - [ Challenges and Learnings](https://www.google.com/search?q=%23-challenges-and-learnings)
  - [ Future Directions](https://www.google.com/search?q=%23-future-directions)
  

-----

##  Dashboards & Visualizations

A series of interactive dashboards were created using Power BI to visualize key insights from the dataset. Below are previews of the dashboards.

#### Overall Patient Health Risk Summary
![Patient Health Risk Insights Dashboard.png](https://github.com/Udaykiran1111/CVD-Risk-Analysis-Prediction/raw/main/cvd%20power%20bi%20and%20ml%20project/Patient%20Health%20Risk%20Insights%20Dashboard.png)

#### CVD Risk Insights by Lifestyle Factors
![CVD Risk Insights.png](https://github.com/Udaykiran1111/CVD-Risk-Analysis-Prediction/raw/main/cvd%20power%20bi%20and%20ml%20project/CVD%20Risk%20Insights.png)

#### Blood Pressure & Cholesterol Analysis
![Blood Pressure & Cholesterol Insights.png](https://github.com/Udaykiran1111/CVD-Risk-Analysis-Prediction/raw/main/cvd%20power%20bi%20and%20ml%20project/Blood%20Pressure%20&%20Cholesterol%20Insights.png)

#### Patient Lifestyle Insights
![Patient Lifestyle Insights.png](https://github.com/Udaykiran1111/CVD-Risk-Analysis-Prediction/raw/main/cvd%20power%20bi%20and%20ml%20project/Patient%20Lifestyle%20Insights.png)

#### Risk Summary and Key Health Indicators
![Patient Risk Summary & Health Indicators.png](https://github.com/Udaykiran1111/CVD-Risk-Analysis-Prediction/raw/main/cvd%20power%20bi%20and%20ml%20project/Patient%20Risk%20Summary%20&%20Health%20Indicators.png)

-----

##  Project Workflow

[cite\_start]The project follows a structured data science pipeline from data ingestion to visualization: [cite: 167]
[cite\_start]`Data Input` → `Preprocessing` → `EDA` → `Modeling` → `Evaluation` → `Dashboard` [cite: 110]

-----

##  Dataset

[cite\_start]The project utilizes the **CAIR-CVD-2025: An Extensive Cardiovascular Disease Risk Assessment Dataset from Bangladesh**, which is publicly available on Mendeley Data. [cite: 22, 11] [cite\_start]The dataset contains detailed demographic, lifestyle, and clinical information for over 500 patients. [cite: 186, 187, 188, 189, 190, 191, 192, 193, 194, 195, 196, 197, 198, 199, 200, 201, 202, 203, 204, 205, 206, 207, 208] [cite\_start]You can find the dataset in this repository (`CVD Dataset.csv`) or download it from the original source. [cite: 28, 183]

-----

##  Technical Stack

[cite\_start]The analysis and modeling were conducted using the following tools and libraries: [cite: 38, 108]

  * [cite\_start]**Programming Language:** Python [cite: 39]
  * [cite\_start]**Data Manipulation:** Pandas, [cite: 40] [cite\_start]NumPy [cite: 41]
  * [cite\_start]**Data Visualization:** Matplotlib, [cite: 42] [cite\_start]Seaborn [cite: 42]
  * [cite\_start]**Statistical Analysis:** SciPy, [cite: 44] statsmodels
  * [cite\_start]**Machine Learning:** Scikit-learn [cite: 43]
  * [cite\_start]**Dashboarding:** Power BI Desktop [cite: 45, 113]
  * [cite\_start]**Development Environment:** Jupyter Notebook [cite: 48, 113]

-----

## ⚙️ Installation & Setup

To replicate this project on your local machine, follow these steps:

1.  **Navigate into the project directory** after downloading.
2.  **Install the required libraries**:
    It is recommended to create a virtual environment first.
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn scipy statsmodels jupyter
    ```
3.  **Ensure you have the dataset** `CVD Dataset.csv` in the root directory of the project.

-----

##  How to Run

The entire data analysis and model building process is documented in the Jupyter Notebook:

1.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2.  Open and run the cells in `eda.ipynb` to see the complete analysis, from data cleaning and EDA to hypothesis testing and model evaluation.
3.  [cite\_start]The interactive dashboards can be viewed by opening the `.pbix` file in Power BI Desktop. [cite: 113]

-----

##  Key Analysis and Results

### Exploratory Data Analysis (EDA)

  * [cite\_start]**Univariate Analysis:** Histograms and boxplots were used to understand the distribution and detect outliers for numerical variables like BMI, BP, and Age. [cite: 120, 121]
  * [cite\_start]**Bivariate Analysis:** Relationships between variables, such as BMI vs. CVD Risk Score, were explored using scatterplots. [cite: 124]
  * [cite\_start]**Correlation Analysis:** A heatmap was generated to identify potential predictors by visualizing the relationships between numerical variables. [cite: 128, 129]

### Hypothesis Testing

  * [cite\_start]A Z-test was conducted to statistically validate differences between high-risk and low-risk patient groups. [cite: 61, 126] [cite\_start]The test revealed a statistically significant difference (p \< 0.0001) in BMI and Systolic BP between the two groups, while Age and Diastolic BP did not show a significant difference. [cite: 132]

### Predictive Modeling

  * [cite\_start]A **Logistic Regression** model was trained to classify patients into high-risk and low-risk categories for CVD. [cite: 132]
  * [cite\_start]The model achieved an overall **accuracy of approximately 93%** on the test set. [cite: 132]
  * [cite\_start]**Model Performance Metrics**: [cite: 132]
      * **Precision:** 0.80 (for the high-risk class)
      * **Recall:** 0.57 (for the high-risk class)
      * **F1-Score:** 0.67 (for the high-risk class)

-----

##  Challenges and Learnings

### Challenges Faced

  * [cite\_start]**Data Quality:** Addressed by implementing a data validation framework and automated quality checks. [cite: 149, 150] [cite\_start]Missing values were handled using median imputation for numerical data and mode for categorical data. [cite: 118, 132]
  * [cite\_start]**Class Imbalance:** The dataset had an imbalance between high-risk and low-risk patients, which was addressed by testing resampling techniques and cost-sensitive learning. [cite: 152, 153, 155]
  * [cite\_start]**Visual Storytelling:** Creating an effective and accessible dashboard required developing user personas and conducting usability testing. [cite: 157, 158]

### Key Learnings

  * [cite\_start]Practical experience in cleaning and preprocessing a real-world healthcare dataset. [cite: 161]
  * [cite\_start]Application of statistical hypothesis testing to validate analytical assumptions. [cite: 162]
  * [cite\_start]Hands-on model evaluation and understanding the trade-offs between metrics like precision and recall in a medical context. [cite: 163, 140]
  * [cite\_start]Proficiency in data storytelling using Power BI to create impactful dashboards. [cite: 164]

-----

##  Future Directions

This project serves as a strong foundation for more advanced predictive systems. Future work could include:

  * [cite\_start]**Time-Series Analysis:** Incorporating time-series data to model disease progression. [cite: 175]
  * [cite\_start]**Integration with Wearable Data:** Integrating data from wearable devices for real-time risk monitoring. [cite: 176]
  * [cite\_start]**EHR Integration:** Exploring the potential for integrating the model with Electronic Health Record (EHR) systems for clinical application. [cite: 171]

-----



##  Contact

If you have any questions or suggestions, feel free to reach out:

**Uday V.**  
 Email: vattikutuudaykiran@gmail.com
