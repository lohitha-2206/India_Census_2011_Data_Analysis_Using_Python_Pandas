# 🇮🇳 India Census 2011 Data Analysis using Python Pandas

## 📌 Project Introduction

This project is based on performing data analysis operations on the India Census 2011 Dataset using Python and the Pandas library inside Jupyter Notebook. The dataset contains information related to population, districts, states, religions, male workers, and various demographic statistics collected during the 2011 Census of India.

The main objective of this project is to understand how Python and Pandas are used in real-world census data analysis for cleaning, formatting, filtering, grouping, and analyzing structured datasets efficiently.

In this project, different data analysis techniques were implemented such as:

- Data Cleaning
- Data Formatting
- Filtering Records
- GroupBy Operations
- Population Analysis
- Religion-wise Population Analysis
- State-wise Analysis
- Exploratory Data Analysis (EDA)

This project provides practical exposure to working with census datasets and understanding how data analysts use Python for extracting meaningful insights from demographic and population data.

---

# 📂 Dataset Information

The dataset contains demographic and population-related records collected during the India Census 2011 survey.

### Dataset Features:

- State_name
- 	District_name
- 	Population
- 	Male
- 	Female
- 	Literate
- 	Workers
- 	Male_Workers
- 	Female_Workers
- 	Cultivator_Workers
- 	Agricultural_Workers
- 	Household_Workers
- 	Hindus
- 	Muslims
- 	Christians
- 	Sikhs
- 	Buddhists
- 	Jains
- 	Secondary_Education	Higher_Education
- 	Graduate_Education
- 	Age_Group_0_29
- 	Age_Group_30_49
- 	Age_Group_50


Each record in the dataset represents census information from a specific district and state in India.

---

# 🛠️ Tools & Technologies Used

## 🐍 Python
Python was used as the programming language for performing data analysis and dataframe operations.

## 📊 Pandas
Pandas library was used for:
- Data Cleaning
- Data Formatting
- Data Manipulation
- Filtering Data
- GroupBy Operations
- Population Analysis

## 📓 Jupyter Notebook
Jupyter Notebook was used to execute Python code interactively and visualize outputs step-by-step.

---

# 🔍 Pandas Functions Implemented

## 🔹 import pandas as pd
Used to import the Pandas library.

### Syntax:
```python
import pandas as pd
```

---

## 🔹 pd.read_csv()
Used to import the CSV dataset into Jupyter Notebook.

### Syntax:
```python
data = pd.read_csv("India_Census_2011.csv")
```

---

## 🔹 style.hide()
Used to hide the dataframe index.

### Syntax:
```python
data.style.hide(axis='index')
```

---

## 🔹 style.set_caption()
Used to set a caption or heading for the dataframe.

### Syntax:
```python
data.style.set_caption("India Census 2011 Data")
```

---

## 🔹 isin()
Used to filter records containing multiple specific values.

### Syntax:
```python
data[data['District_name'].isin(['New Delhi', 'Lucknow', 'Jaipur'])]
```

---

## 🔹 groupby()
Groups data according to a specific column.

### Syntax:
```python
data.groupby('State_name')['Population'].sum()
```

---

## 🔹 Filtering Records
Used to access records based on specific conditions.

### Syntax:
```python
data[data.State_name == 'Maharashtra']['Male_Workers']
```

---

## 🔹 set_index()
Used to set a specific column as the dataframe index.

### Syntax:
```python
data.set_index('State_name')
```

---

## 🔹 add_prefix()
Adds a prefix to all column names.

### Syntax:
```python
data.add_prefix('value_')
```

---

## 🔹 add_suffix()
Adds a suffix to all column names.

### Syntax:
```python
data.add_suffix('_value')
```

---

# 📊 Tasks Performed in the Project

## ✅ Q1) Hiding DataFrame Index

### Task:
Hide the indexes of the dataframe.

### Code Used:
```python
data.style.hide(axis='index')
```

### Explanation:
- Removes dataframe indexes from display
- Makes dataframe output cleaner and more professional

---

# 📊 Q2) Setting Caption on DataFrame

### Task:
Set a caption or heading on the dataframe.

### Code Used:
```python
data.style.set_caption("India Census 2011 Data")
```

### Explanation:
- Adds a descriptive heading to the dataframe
- Improves readability and presentation

---

# 📊 Q3) Filtering District Records

### Task:
Show records related to New Delhi, Lucknow, and Jaipur districts.

### Code Used:
```python
data[data['District_name'].isin(['New Delhi', 'Lucknow', 'Jaipur'])]
```

### Explanation:
- Filters records of selected districts
- Useful for targeted district-level analysis

---

# 📊 Q4) State-wise Population Analysis

### Task:
Calculate state-wise total population and religion-wise population.

### Code Used:
```python
data.groupby('State_name')['Population'].sum()

data.groupby('State_name')[['Hindus', 'Muslims', 'Christians', 'Sikhs', 'Buddhists', 'Jains']].sum()
```

### Explanation:
- Groups records by state
- Calculates total population statistics
- Helps compare religious demographics state-wise

---

# 📊 Q5) Male Workers Analysis

### Task:
Find the total number of Male Workers in Maharashtra.

### Code Used:
```python
data[data.State_name == 'Maharashtra']['Male_Workers']
```

### Explanation:
- Filters records related to Maharashtra
- Displays male worker statistics

---

# 📊 Q6) Setting Index

### Task:
Set a column as the index of the dataframe.

### Code Used:
```python
data.set_index('State_name')
```

### Explanation:
- Converts a selected column into dataframe index
- Helps organize and access data efficiently

---

# 📊 Q7) Adding Prefix & Suffix

### Task:
Add prefix and suffix to dataframe column names.

### Code Used:
```python
data.add_prefix('value_')

data.add_suffix('_value')
```

### Explanation:
- Modifies column names by adding custom text
- Useful for formatting and dataset customization

---

# 📌 Important Insights

✔️ Pandas makes census data analysis simple and efficient.

✔️ GroupBy operations help compare population statistics state-wise.

✔️ Filtering records allows district-level demographic analysis.

✔️ Data formatting functions improve dataframe presentation.

✔️ Population and religion-wise analysis help understand demographic distributions.

✔️ Real-world census datasets can be analyzed efficiently using Python.

---

# 📁 Project Structure

```text
├── India_Census_2011_Data_Analysis.ipynb
├── Census_Data.csv
├── README.md
```

---

# 🎯 Final Conclusion

This project demonstrates how Python and Pandas can be used for real-world census data analysis and preprocessing tasks. Different operations such as filtering records, grouping data, formatting dataframes, population analysis, and extracting meaningful insights were successfully implemented.

Through this project, practical understanding was gained in:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Manipulation using Pandas
- GroupBy Operations
- Population Analysis
- Data Formatting
- Python-based Data Analytics

Overall, this project serves as a strong beginner-friendly foundation for learning Data Analysis and Data Science using Python.
