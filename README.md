# 📚 Student Exam Scores - Exploratory Data Analysis (EDA)

<p align="center">
  This project performs an in-depth exploratory data analysis (EDA) on a dataset containing student exam scores and various factors that might influence academic performance.
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.7%2B-blue" alt="Python Version">
  <img src="https://img.shields.io/badge/Pandas-lightgrey" alt="Pandas">
  <img src="https://img.shields.io/badge/Matplotlib-red" alt="Matplotlib">
  <img src="https://img.shields.io/badge/Seaborn-blueviolet" alt="Seaborn">
</p>

---

## 📊 Overview

The analysis explores relationships between **study habits**, **sleep patterns**, **attendance**, **previous academic performance**, and final exam results. This project demonstrates a complete EDA workflow from data ingestion to visualization and key insights.

---

## 📁 Dataset Information

The dataset contains **200 student records** with the following features:

* `student_id`: Unique identifier for each student
* `hours_studied`: Number of hours studied for the exam
* `sleep_hours`: Number of hours slept the night before the exam
* `attendance_percent`: Percentage of classes attended
* `previous_scores`: Scores from previous exams
* `exam_score`: The target variable - final exam score

---

## 🗂️ Project Structure

student-exam-scores-eda/

├── data/

   └── student_exam_scores.csv          # 📥 Raw dataset

├── notebooks/

   └── student_exam_scores_eda.ipynb    # 📝 Complete EDA analysis

├── reports/

   └── figures/                         # 🖼️ Generated visualizations

│       ├── correlation_matrix.png

│       ├── feature_distributions.png

│       ├── pairplot.png

│       └── scatter_matrix.png

├── README.md                            # 📄 Project documentation

├── requirements.txt                     # 📦 Python dependencies

└── .gitignore                           # 🚫 Git ignore rules

---

## 🚀 Installation & Setup

1.  **Clone the repository**
    ```bash
    git clone <repository-url>
    cd student-exam-scores-eda
    ```
2.  **Install required packages**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Launch Jupyter Notebook**
    ```bash
    jupyter notebook notebooks/student_exam_scores_eda.ipynb
    ```

---

## 📈 Key Findings

### **Correlation Analysis**

* **Strong positive correlation** (0.89) between `previous_scores` and `exam_score`.
* **Moderate positive correlation** (0.63) between `hours_studied` and `exam_score`.
* **Weak positive correlation** (0.24) between `attendance_percent` and `exam_score`.
* **Minimal correlation** between `sleep_hours` and `exam_score`.

### **Top vs Bottom Performers**

| Metric | Top 10 Performers | Bottom 10 Performers |
| :--- | :---: | :---: |
| **Hours Studied** | **9.8 hours** | **2.0 hours** |
| **Attendance** | **84.5%** | **63.6%** |
| **Previous Scores** | **83.4** | **50.9** |

### **Optimal Ranges**

* **Sleep**: **7-9 hours** showed best performance (average score: 34.8).
* **Study time**: **6-9 hours** optimal (average score: 36.8).
* **Attendance**: **>90%** showed best results (average score: 36.2).

---

## 🔍 Analysis Techniques & Visualizations

**Techniques Used:**
* Descriptive Statistics
* Correlation Analysis
* Outlier Detection
* Categorical Binning
* Comparative Analysis

**Visualizations Included:**
* **Correlation matrix heatmap** 🌡️
* **Feature distribution histograms** 📊
* **Pairplot** of all numerical features 📈
* **Box plots** for outlier detection 📦

---

## 📋 Data Quality

* ✅ **No missing values** found.
* ✅ **No duplicate records** identified.
* ✅ All data types and ranges are appropriate.

---

## 🎯 Potential Applications

* **Educational Institutions**: Use insights to improve student performance.
* **Students**: Optimize study habits based on data-driven recommendations.
* **Researchers**: Build predictive models for student performance.
* **Educators**: Identify at-risk students early.

---

## 🛠️ Dependencies

* Python 3.7+
* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* jupyter

