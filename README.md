# Data Analysis Project with Python
## Crime Data Analysis of India 2020

A Python-based data analysis project using **Jupyter Notebook** to explore the *NCRB Crime in India 2020* dataset. This project covers data cleaning, exploratory data analysis (EDA), and data visualization using **Pandas**, **Matplotlib**, and **Seaborn**.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset Description](#-dataset-description)
- [Key Questions Answered (Q&A)](#-key-questions-answered-qa)
- [Prerequisites](#️-prerequisites)
- [Installation](#-installation)
- [How to Run](#-how-to-run)
- [Tools & Libraries Used](#-tools-and-libraries-used)

---

# 📈 Project Overview

This project analyzes crime trends across India using official NCRB data from 2020. The goal is to:
- Clean and preprocess real-world data
- Explore state-wise and crime-wise statistics
- Visualize key insights using bar charts, heatmaps, and more
- Understand regional trends and anomalies

The Jupyter Notebook walks through the entire pipeline of data analysis from import to insight.

---

# 🗂 Dataset Description

The dataset used is published by the **National Crime Records Bureau (NCRB), Ministry of Home Affairs, India**, and contains detailed records of reported crimes across Indian states and union territories for the year 2020.

Key features:
- Crime statistics by age
- State/UT-wise distribution
- Gender based breakdowns

> **Source:** [ncrb.gov.in](https://ncrb.gov.in)

---

## ❓ Key Questions Answered (Q&A)

| # | Analytical Question / Objective | Key Finding |
|---|---|---|
| **1** | **Which cities report the highest crime numbers?** | Metropolitan hubs like Delhi lead total reported offenses by a notable margin. |
| **2** | **What is the gender distribution of offenders?** | ~80% male vs. ~20% female; female offenders show sharp concentrations in specific cities. |
| **3** | **Which age demographic is most prone to crime?** | Young adults aged **18–30** account for the largest share (>45%), followed by 30–45. |
| **4** | **What is the extent of juvenile offenses?** | Juveniles comprise ~6% of total crimes overall, but exceed 10% in select high-risk cities. |
| **5** | **Which cities cross high female crime thresholds?** | Cities with >10,000 total crimes and >1,000 female crimes were filtered and analyzed. |
| **6** | **Does female crime correlate with male crime?** | Scatter plot analysis confirms a positive linear correlation between male and female crime volumes across cities. |

> 📄 For in-depth methodology, breakdown, and query logic, see [**QA.md**](QA.md).

---

## ⚙️ Prerequisites

Before running this project, ensure you have the following installed:

- Python 3.7+
- Jupyter Notebook
- pip (Python package manager)

Required Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- openpyxl (for reading `.xlsx` files)

You can install them via:
```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

---

## 🛠 Installation

**1. Clone the repository:**
```bash
git clone https://github.com/ayushgupta-120/Data-Analysis-Project.git
cd Data-Analysis-Project
```

**2. (Optional) Create a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

**3. Install dependencies:**
```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

---

## 🚀 How to Run

**1. Launch Jupyter Notebook:**
```bash
jupyter notebook
```

**2. Open the file:**
`Data_Analysis_Project_with_Python.ipynb`

**3. Run each cell step-by-step to follow the analysis.**

---

## 📊 Tools and Libraries Used
- Python – Core programming language
- Jupyter Notebook – Interactive coding environment
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Plotting and visualizations
- Seaborn – Statistical data visualization

---

### Screenshots

![image](https://github.com/user-attachments/assets/c8c2ba43-ea80-4bd3-a918-4d2786c68056)

![image](https://github.com/user-attachments/assets/c3fe0f4f-45e9-45f9-9d37-539d76d38e7e)
