# EDA-project
Exploratory Data Analysis (EDA) is the process of analyzing and summarizing datasets using statistical methods and visualizations to understand their structure, detect patterns, identify anomalies, and prepare data for modeling.  it is typically the first major step in any data science, machine learning, or analytics project. 

The Project Title: Exploratory Data Analysis
📊 Exploratory Data Analysis (EDA) Module

Welcome to the "EDA Module Project"! 🚀
This project demonstrates how to perform "data cleaning", "data analysis", and "data visualization" using Python libraries. It works on a dataset called "dirty_dataset.csv" and transforms it into a cleaner, more understandable format through Exploratory Data Analysis (EDA).



🧾 Project Overview:

This project focuses on:
* Loading a dataset
* Identifying missing values
* Cleaning and preprocessing data
* Performing statistical analysis
* Visualizing relationships between variables
* Generating insights using charts and graphs
EDA is an essential step before building machine learning models or making data-driven decisions.



🎯 Objectives:
* Understand the structure of the dataset
* Handle missing values effectively
* Explore relationships between variables
* Detect patterns and trends
* Visualize data using multiple chart types
* Prepare data for further analysis or modeling


📂 Dataset Used"
File Name : "dirty_dataset.csv"

The dataset contains customer-related information such as:
* Age
* Income
* Education
* Marital Status
* Loan Amount
* Average Monthly Spend
Some values in the dataset are missing, making it suitable for demonstrating data cleaning techniques.



🛠️ Technologies & Libraries Used

* "Python" 🐍
* "Pandas" – Data manipulation
* "NumPy"– Numerical operations
* "Matplotlib" – Basic plotting
* "Seaborn" – Statistical visualization
* "Plotly" – Interactive visualization



🔍 Steps Performed in the Project

1️⃣ Import Libraries
The project starts by importing required Python libraries for data analysis and visualization.

2️⃣ Load Dataset
The dataset is loaded using:
python:
df = pd.read_csv("dirty_dataset.csv")


3️⃣ Data Exploration
Basic dataset inspection is performed using:

* "df.head()" – View first rows
* "df.describe()" – Summary statistics
* "df.info()" – Data structure
* "df.isnull().sum()" – Missing values check



4️⃣ Data Cleaning 🧹
Missing values are handled using:
* "Mean" for numerical columns
* "Mode" for categorical columns

Columns cleaned:
* Age
* Income
* Education
* Marital Status
* Loan Amount
* Average Monthly Spend

Example:
python:
df['age'] = df['age'].fillna(df['age'].mean())




📊 Data Visualization
The project includes several visualizations to understand the dataset better.

📈 Histogram
Shows distribution of education levels.
python:
sns.histplot(x=df['education'], kde=True)




📦 Box Plot
Displays relationship between:
* Age
* Marital Status
python:
sns.boxplot(x=df['age'], y=df['marital_status'])




🔵 Scatter Plot
Shows relationship between:
* Age
* Income
* Education
python:
sns.scatterplot(x=df['age'], y=df['income'], hue=df['education'])




📊 Bar Plot
Compares:
* Income
* Age
python:
sns.barplot(x=df['income'], y=df['age'])



📉 Line Plot
Displays relationship between:
* Average Monthly Spend
* Loan Amount
python:
sns.lineplot(x=df['avg_monthly_spend'], y=df['loan_amount'])




🔥 Correlation Heatmap
Shows correlation between numerical variables.
python:
corr = df.corr(numeric_only=True)
sns.heatmap(corr, annot=True)




🥧 Interactive Pie Chart
Created using Plotly for interactive visualization.
python:
fig = px.pie(df, values='age', names='income', title='Interactive EDA Pie')
fig.show()




📦 Project Features
✅ Data Cleaning
✅ Missing Value Handling
✅ Statistical Summary
✅ Multiple Visualizations
✅ Correlation Analysis
✅ Interactive Charts
✅ Beginner-Friendly EDA Workflow



▶️ How to Run the Project
1. Install required libraries:

bash
pip install pandas numpy matplotlib seaborn plotly


2. Place the dataset file:
dirty_dataset.csv


3. Run the Python script:
bash
python edamodule_315.py



📌 Expected Output:
After running the project, you will get:

* Cleaned dataset
* Summary statistics
* Visualizations (charts and graphs)
* Correlation heatmap
* Interactive pie chart
* Better understanding of the dataset





**Happy Learning & Data Exploring! 📊🚀**
