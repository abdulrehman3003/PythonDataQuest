# Python DataQuest Competition - Day 4

## Objective
This project is part of the Python DataQuest Competition, which involves completing three data manipulation tasks using Python libraries like Pandas, Matplotlib, and the CSV module. The tasks focus on data analysis, cleaning, visualization, and handling CSV files within a 2-hour timeframe.

## Task Breakdown

### Task 1: Data Analysis and Visualization (Pandas + Matplotlib)
**Objective:** Analyze and visualize a dataset to generate meaningful insights.

#### Steps:
1. **Convert Date Column:**
   - Convert the `dteday` column to a proper date format using:
     ```python
     df['dteday'] = pd.to_datetime(df['dteday'])
     ```
2. **Data Analysis and Visualization:**
   - Analyze trends, distributions, and correlations in the dataset.
   - Suggested visualizations:
     - Time-series plots for changes over time.
     - Histograms or bar charts for distributions.
     - Scatter plots for relationships between variables.
3. **Reporting:**
   - Summarize findings and support them with visualizations.

### Task 2: Data Cleaning and Transformation (Pandas)
**Objective:** Clean and transform data, including calculating artist ages.

#### Steps:
1. **Clean Nationality and Gender Columns:**
   - Remove unwanted characters like parentheses.

2. **Clean and Convert Date Columns:**
   - Remove unwanted characters from `BeginData` and `EndDate`.
   - Convert these columns to integers, handling missing or bad data.
   - Calculate `actual_age` as:
     ```python
     df['actual_age'] = df['EndDate'] - df['BeginData']
     ```
   - Use a placeholder value (e.g., `"-"`) for missing data.

3. **Clean Submission Date Column:**
   - Remove bad characters for accurate calculations.

### Task 3: Data Handling with CSV (Python's `csv` Library)
**Objective:** Clean and organize account transaction data.

#### Steps:
1. **Extract Account Names:**
   - Read the CSV file and associate each transaction with its corresponding account name.

2. **Remove Total Rows:**
   - Filter out rows containing totals by identifying specific keywords (e.g., "Total").

3. **Remove Irrelevant Rows:**
   - Remove rows where the `Date` column contains "Beginning Balance."

## Collaboration and Task Management
- **Teamwork:** Efficient task division and collaboration are crucial for completing the tasks within the given timeframe.
- **Skills Utilization:** Leverage individual strengths for data analysis, visualization, and data handling.

## Tools and Libraries
- **Pandas:** For data manipulation and cleaning.
- **Matplotlib:** For data visualization.
- **CSV Module:** For handling CSV files.

## Learning Objectives
- Gain practical experience in data analysis and visualization.
- Develop data cleaning and transformation skills.
- Learn effective CSV data handling techniques.

## Disclaimer
This project is for educational purposes as part of the DataQuest Competition.

