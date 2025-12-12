# MSCS 634 Comprehensive Data Mining Project
## Bank Marketing Prediction Analysis
### Project Overview
This repository contains the complete analysis of the Bank Marketing dataset from the UCI Machine Learning Repository. The primary goal of this project was to apply advanced data mining techniques to predict whether a customer will subscribe to a term deposit. By processing raw data through a structured pipeline of cleaning, feature engineering, and modeling, this project provides actionable insights to optimize marketing campaigns and improve conversion rates.

The project was executed in four phases, evolving from exploratory analysis to complex predictive modeling and unsupervised learning pattern discovery.

### Dataset
The dataset relates to the direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be subscribed or not.

  - Source: UCI Machine Learning Repository
  - Records: 41,176
  - Features: 20 input variables including client demographics, financial standing, and macroeconomic indicators.
  - Target: Binary classification (yes or no) for term deposit subscription.

### Project Roadmap
#### Phase 1: Data Preparation and Exploration
The initial phase established a clean baseline for analysis. Key tasks included handling missing values such as the specific code used for clients who had never been contacted before. Categorical variables with unknown values were managed to preserve information. Exploratory data analysis was conducted to understand feature distributions and remove attributes that would cause data leakage.

#### Phase 2: Regression Modeling
This phase focused on estimating the likelihood of a customer subscribing using regression algorithms. Feature engineering was performed to create binned variables for age and campaign frequency. Linear Regression and Ridge Regression models were trained and evaluated. The results indicated that while regression provided a baseline for feature importance, the problem was better suited for classification techniques.

#### Phase 3: Classification and Pattern Discovery
The core modeling phase involved building classifiers to predict the binary subscription outcome. Decision Trees and Random Forest classifiers were developed and tuned. The Random Forest model achieved superior performance with an ROC AUC score of 0.79. Additionally, unsupervised learning techniques were applied. K-Means clustering identified three distinct customer personas, and Apriori association rule mining revealed frequent patterns linking job types to education levels.

#### Phase 4: Final Synthesis
The final phase consolidated all findings into strategic business recommendations. This included strategies for targeting specific demographics and optimizing call frequencies. Ethical considerations regarding algorithmic fairness and data privacy were also addressed to ensure responsible deployment of the models.

### Repository Structure
  - **MSCS_634_Project.ipynb:** The consolidated Jupyter Notebook containing all code for data cleaning, EDA, regression, classification, clustering, and association rule mining.
  - **bank_marketing_clean_baseline.csv:** The processed dataset used for modeling.
  - **Project_Report.pdf:** The comprehensive written report detailing methodology, results, and recommendations.
  - **Presentation_Slides:** The slides used for the video presentation.

### Findings
  - **Best Model:** The Tuned Random Forest Classifier provided the most reliable predictions, significantly reducing false positives compared to other models.
  - **Customer Segments:** Clustering revealed three primary groups comprising cold leads, standard clients, and high propensity targets.
  - **Strategic Insight:** Association rules highlighted that technicians with professional course education form a distinct and responsive demographic.
  - **Campaign Efficiency:** Analysis showed that increasing contact frequency beyond a certain point yields diminishing returns, suggesting a cap on the number of calls per client.

### Technologies Used
  - Python
  - Pandas
  - NumPy
  - Scikit-learn
  - Matplotlib
  - Seaborn
  - Mlxtend
