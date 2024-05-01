# ML_Project9-StudentPerformanceAnalysis

### Student Performance Analysis Project
This repository contains the code and analysis for a comprehensive study of student performance data. We utilize various libraries like pandas, numpy, matplotlib, seaborn, and plotly to explore and analyze the data from the "StudentsPerformance.csv" file.

### Key Objectives:

##### 1.Data Loading and Inspection:
```
Libraries like pandas, numpy, matplotlib, seaborn, and plotly are imported for data manipulation and visualization.
The CSV file "StudentsPerformance.csv" is loaded using pandas.
The data shape is checked, revealing 1000 rows and 8 columns.
The head() function displays the first few rows to get a glimpse of the data.
describe() provides summary statistics for numerical columns (mean, standard deviation, min, max).
select_dtypes('object') shows the number of unique items present in categorical columns.
isnull().sum() checks for missing values, revealing no missing data in this dataset.
```

##### 2.Descriptive Statistics and Inferential Statistics:
```
dabl.plot is used to create various plots comparing each attribute with the target scores (math, reading, writing). This helps visualize potential relationships.
The probability of students scoring above 50 in each subject is calculated, indicating that students are more likely to score above 50 in reading (90.3%) and writing (87.6%) compared to math (85%).
The probability of students passing all three subjects with a score above 40 is calculated to be 93.90%.
Similarly, the probability of scoring above 90 in all subjects is calculated to be a much lower 2.30%.
Skewness is checked for the target columns, revealing no significant skewness.
```

##### 3.Confidence Intervals:
```
Confidence intervals are calculated for the mean scores of math, reading, and writing using the scipy.stats library.
The intervals represent a range within which the true population mean is likely to fall with a certain level of confidence (95% in this case).
```

##### 3.Grouping Operations:
```
The number of girls scoring 90+ in all subjects is retrieved using boolean indexing.
Data is grouped by gender and various attributes like lunch, test preparation course, and race/ethnicity to compare median scores and identify potential patterns.
```

##### 4.Data Visualizations:
```
Count plots are created using seaborn to visualize the distribution of categorical variables like gender, race/ethnicity, parental education level, lunch type, and test preparation course.
Distribution plots are created for math, reading, and writing scores to understand their spread.
Additional visualizations compare different categorical variables like gender vs race/ethnicity, race/ethnicity vs parental education level, etc., to uncover potential relationships.
```

##### 5.Feature Engineering (Example):
```
A new column "pass_math" is created to indicate whether students passed the math exam based on a set passing mark (40 in this case). Similar columns can be created for other subjects.
```

### Project Highlights:

The code provides a comprehensive overview of the data, including descriptive statistics, probability calculations, confidence intervals, and visualizations.

Grouping operations allow for targeted analysis based on specific demographics and student characteristics.

The example of creating a "pass_math" feature demonstrates the potential for further feature engineering to extract deeper insights.


### Further Exploration:

Building machine learning models to predict student performance based on various attributes.

Performing in-depth analysis on specific relationships identified through visualizations.

Creating additional feature engineering techniques to extract more insights from the data.

### Additional Notes:

This is a basic framework for student performance analysis. You can customize and extend the code to explore specific research questions or delve deeper into specific areas of interest.

Feel free to contribute to this project by adding new analysis techniques, visualizations, or insights.
