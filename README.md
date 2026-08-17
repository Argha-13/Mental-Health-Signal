# Mental Health Score Predictor

## Overview
This project involves a machine learning pipeline designed to analyze and predict a student's `Mental_Health_Score` based on their social media habits, lifestyle choices, and academic routines. The repository currently contains the Exploratory Data Analysis (EDA) step, highlighting key lifestyle trends and their correlations with mental well-being.

---

## Dataset Details
The model leverages the `Student Social Media And Mental Health Impact.csv` dataset. 

*   **Size**: The dataset contains exactly 5000 records.
*   **Total Features**: There are 13 columns (5 float, 2 integer, 6 object/categorical).
*   **Numerical Features**: Age, Avg_Daily_Usage_Hours, Daily_Unlocks, Study_Hours, Physical_Activity_Hours, Sleep_Hours_Per_Night, and Mental_Health_Score.
*   **Categorical Features**: Gender, Country, Academic_Level, Most_Used_Platform, Purpose_Of_Use, and Stress_Level.

### Target Variable
*   **`Mental_Health_Score`**: A continuous numerical scale (ranging from 3.6 to 9.4 in this dataset) representing the overall mental well-being of the student. 

---

## Exploratory Data Analysis (EDA)
Initial data exploration reveals critical insights into how different variables interact with a student's mental health. Key visualizations generated in this phase include:

*   **Distribution Analysis**: A histogram mapping the distribution and frequency of the `Mental_Health_Score` across the 5000 students.
*   **Correlation Tracking**: A numeric heatmap showing the correlation coefficients between all continuous variables to isolate the strongest predictors.
*   **Stress Level vs. Mental Health**: A boxplot mapping the categorical `Stress_Level` (Low, Medium, High, Very High) against the continuous `Mental_Health_Score`.
*   **Usage vs. Well-being**: A scatterplot visualizing the relationship between `Avg_Daily_Usage_Hours` and `Mental_Health_Score`.

### Visual Findings
Below are key snapshots from the visualization phase:

![Correlation Heatmap](image_2157c5.jpg)

![Scatterplot Analysis](image_2157c0.jpg)

---

## Tech Stack & Libraries
This analysis and modeling pipeline utilizes the following Python libraries:
*   **NumPy**: Numerical computing and array manipulation.
*   **Pandas**: Data manipulation and CSV ingestion.
*   **Matplotlib & Seaborn**: Data visualization and plotting (heatmaps, boxplots, scatterplots).

---

## Getting Started

### Prerequisites
Ensure you have Python 3.7+ installed along with the required libraries. 
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Usage
1. Clone the repository.
2. Ensure `Student Social Media And Mental Health Impact.csv` is in the root directory.
3. Run the Jupyter Notebook to view the EDA and execute the model training cells.

## Next Steps / Roadmap
1. **Data Preprocessing**: Encode categorical variables (e.g., one-hot encoding for `Most_Used_Platform`, ordinal encoding for `Stress_Level`).
2. **Model Selection**: Train regression models (e.g., Random Forest, XGBoost, Linear Regression) to predict the `Mental_Health_Score`.
3. **Evaluation**: Measure model performance using metrics like RMSE (Root Mean Squared Error) and R-squared.

Usage
Clone the repository.

Ensure Student Social Media And Mental Health Impact.csv is in the root directory.

Run the Jupyter Notebook to view the EDA and execute the model training cells.

Next Steps / Roadmap
Data Preprocessing: Encode categorical variables (e.g., one-hot encoding for Most_Used_Platform, ordinal encoding for Stress_Level).

Model Selection: Train regression models (e.g., Random Forest, XGBoost, Linear Regression) to predict the Mental_Health_Score.

Evaluation: Measure model performance using metrics like RMSE (Root Mean Squared Error) and R-squared.
