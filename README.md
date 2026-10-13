# Titanic Dataset Analysis and Exploratory Data Analysis (EDA)

## Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** of the Titanic dataset using Python. The main objective is to explore passenger information, handle missing values, understand data distributions, and identify factors associated with passenger survival.

The project uses data analysis libraries to clean, summarize, and visualize the dataset through different statistical techniques and charts.

## Objectives

- Load and explore the Titanic dataset.
- Understand the structure and characteristics of the data.
- Identify and handle missing values.
- Convert columns into appropriate data types.
- Perform descriptive statistical analysis.
- Create univariate, bivariate, and multivariate visualizations.
- Study relationships between passenger survival and other features.
- Draw meaningful insights from the dataset.

## Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Jupyter Notebook** — Interactive development environment

## Dataset

The project uses the Titanic dataset available through Seaborn.

The dataset contains information about passengers aboard the Titanic, including:

- `survived` — Survival status (0 = No, 1 = Yes)
- `pclass` — Passenger class
- `sex` — Passenger gender
- `age` — Passenger age
- `sibsp` — Number of siblings or spouses aboard
- `parch` — Number of parents or children aboard
- `fare` — Passenger fare
- `embarked` — Port of embarkation
- `deck` — Passenger deck information
- `class` — Passenger class category

The dataset contains **891 rows and 15 columns** before data cleaning.

## Project Workflow

### 1. Importing Libraries

The project imports Pandas, NumPy, Matplotlib, and Seaborn to perform data manipulation, numerical operations, and visualization.

### 2. Loading the Dataset

The Titanic dataset is loaded using Seaborn and converted into a Pandas DataFrame.

The dataset is explored using:

- `head()` — View the first rows
- `tail()` — View the last rows
- `shape` — Check the number of rows and columns
- `columns` — Display column names
- `info()` — Inspect data types and non-null values

### 3. Data Cleaning

The dataset is checked for missing values.

The notebook includes these data-cleaning operations:

- Filling missing values in the `embarked` column with its mode.
- Filling missing values in the `deck` column with `"C"`.
- Filling missing values in the `age` column with the mean age.
- Checking missing values after the cleaning operations.

### 4. Data Type Conversion

Selected columns are converted into appropriate data types for analysis.

These include:

- `survived` — Category
- `pclass` — Category
- `sex` — Category
- `age` — Integer
- `embarked` — Category

### 5. Descriptive Statistics

Descriptive statistics are generated using Pandas to understand the numerical data.

The analysis uses statistical summaries to examine values such as the mean, standard deviation, minimum, maximum, and quartiles.

### 6. Univariate Analysis

Univariate analysis examines individual variables separately.

Visualizations include:

- Age distribution histogram
- Passenger survival count
- Passenger class distribution
- Gender distribution
- Siblings and spouses distribution
- Parents and children distribution
- Embarkation port distribution
- Age box plot
- Age distribution density plot

### 7. Bivariate Analysis

Bivariate analysis explores relationships between two variables.

The notebook examines:

- Passenger gender and survival
- Passenger age and survival
- Passenger embarkation port and survival
- Passenger age and fare

These visualizations help identify differences in survival outcomes across passenger groups.

### 8. Multivariate Analysis

Multivariate analysis explores patterns involving multiple variables.

The project includes:

- Survival by passenger class
- Survival by gender
- Age distribution by survival status
- Fare and age scatter plots
- Correlation heatmap
- Passenger class pie chart
- Combined visualizations comparing survival, class, gender, age, and fare

## Key Insights

The analysis highlights the following patterns:

- **Gender:** Women had a higher survival rate than men.
- **Passenger Class:** First-class passengers generally had better survival outcomes than passengers in lower classes.
- **Age:** Younger passengers showed some survival advantages, although age alone did not determine survival.
- **Fare:** Higher fares were associated with passenger groups that generally experienced better survival outcomes.
- **Embarkation Port:** Southampton was the most common embarkation port, and survival outcomes varied across ports.
- **Family Size:** Traveling with family members had mixed effects on survival.

These findings describe associations observed in the dataset and do not establish that any single feature caused survival.

## Visualizations

The project uses several types of charts to make the analysis easier to understand:

- Histograms
- Count plots
- Box plots
- Scatter plots
- Pie charts
- Bar charts
- Correlation heatmaps
- Combined subplot visualizations

## Installation and Setup

### Prerequisites

Install Python and Jupyter Notebook on your computer.

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### Step 2: Open the Project Folder

```bash
cd YOUR_PROJECT_FOLDER
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Step 4: Start Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Notebook

Open `Final_Project.ipynb` and execute the cells from top to bottom.

**Note:** The notebook loads the Titanic dataset through Seaborn. An internet connection may be required if the dataset is not already cached locally.

## Project Structure

```text
Titanic-Dataset-Analysis/
│
├── Final_Project.ipynb
└── README.md
```

## Conclusion

This project demonstrates how Python can be used to perform exploratory data analysis on a real-world dataset.

By cleaning the data, examining statistical summaries, and creating visualizations, the project identifies important patterns related to Titanic passenger survival.

The analysis suggests that gender, passenger class, age, fare, and family circumstances were associated with different survival outcomes.

Overall, this project provides practical experience in data cleaning, data exploration, statistical analysis, and visualization using Python.

## Future Improvements

- Improve the missing-value treatment using more detailed analysis.
- Compare survival rates using percentages instead of counts alone.
- Perform deeper statistical analysis of passenger characteristics.
- Build a machine learning model to predict passenger survival.
- Evaluate a prediction model using suitable classification metrics.

## Author

NIDHESH DUBEDI.

## License

This project is intended for educational and learning purposes.
