# Sales Exploratory Data Analysis with Python

* **To view a pdf version of the project, click here**
* **To view the jupyternotebook, click here**

## PROJECT SUMMARY

### OBJECTIVES
This project focuses on applying Exploratory Data Analysis (EDA) on the sales data of a fictitous company in order to acheive the following:
> * investigate and understand the data
> * identify the distribution of the data
> * summarize the main characteristics of the data
> * detect outliers and anomalies
> * establish relationships between the variables
> * visualization of the data

Exploring the data also helps to answer some questions:
> * What
> * What
> * What
> 
**The overall aim of conducting EDA on the sales data is to discover transactional patterns and gain insights which would help the sales and marketing team make better decisions, thereby improving sales performance and profits.**

### TOOLS
The main tool used for this project is **Python**. The following Python Libraries are used for the project:
> * **Pandas**
> * **NumPy**
> * **Matplotlib**
> * **Seaborn**
> * **Plotly**
> * **wordCloud**


### PROCEDURE
The project is broken down into the following steps:

### Step 1: Overview and summary of the data:
 Here the focus is to have a glimpse of the data to see its size, types, missing values, summary statistics and columns. 
    To do this, the following functions and methods were used:
    * .head() 
    * .tail()
    * .info()
    * .describe()
    * .size()
    * .columns
    * .shape
    * .dtypes
    * .isnull()
 **Conclusion:**
 * There were no missing values in the sales data set.
 * The dataset had 13 columns
 * The dataset had 113035 rows of data
 * The date column was not in the correct datatype 'datetime'
   
  
 ### Step 2: Data Cleaning and Preparation
 The data did not need much cleaning. However, some new columns had to be created
 * Conversion of date column from object to datetime
 * Extraction of the Year, Month and Day from the Date column and creating new columns for them
 * Calculation of Total sales and Profit and creating 2 new columns for the results
  
  ### Step 3: Checking the unique values in each column to answer the following questions:
 * What is the customer demographic, in terms of age?
 * What countries and states do the company serve?
 * What products do the company sell?
 * How are the products categorised?
   
  
  ### Step 4:  UNIVARIATE ANALYSIS
  Univariate analysis is the most basic form of analysis. It takes into consideration one variable at a time. The aim of univariate analysis is to understand the distribution of data in a dataset. Univariate analysis can be both graphical and non-graphical. For the purpose of this project, both types of univariate analysis would be conducted. 

**Non-Graphical Univariate Analysis:**

**Measure of Central Tendency and Dispersion**
   * The first type of univariate analysis conducted is the non-graphical univariate analysis.
   * Since the company's major focus is sales, the target variable in the analysis is 'Sales'. The Central tendency and dispersion of the sales variable is checked.
      Central tendency is a statistical measure which identifies a single value as representation of an entire distribution. The mean is the most common central             tendency and for this sales variable, the mean is used as the central tendency. Dispersion shows the distribution or spread of the data and the most common             measures of dispersion are standard deviation, variance and interquartile range. 
   * Using the **describe() method, the central tendency and dispersion are identified.**
  
  **Measure of Skewness**
  The statistical measures that show the shape of the distribution of the data are skewness and kurtosis. Skewness is a measure of asymetry: it defines the extent to which a distribution differs from normal distribution. A distribution may have a right(positive) skewness or a left(negative) skewness or zero skewness. 
  * Positive skewness means the data is skewed to the right, the data is concentrated to the right and the value is poitive. mean > median > mode.
  * Negative skewness means the data is skewed to the left, the data concentration is on the left and the value is negative. mean < median < mode.
  * Zero skewness means the data is symmetrical and the distibution is normal. It is depicted by zero. mean = median = mode
  * Skewness between -0.5 and 0.5 means the data is fairly symmetrical.
  * Skewness between -1 and 0.5 means the data is moderately skewed.
  * Skewness less than -1 or greater than 1 means the data is highly skewed.
  * Using the .skew() function, the distribution of the data is given, in terms of skewness
   
  | **Observation** |
  | --------------  |
  | * The minimum sales value is 2, the maximum sales value is 69136 and the count is 113036. |
  | * The measure of dispersion(standard deviation) is 1466.202934. |
  | * The central tendency given by the mean is 842 and given by the median is 245. |
  | * IQR is the difference between the 75th and 25th percentile, and the IQR for the sales variable is 810 |
  | * The skewness of the sales variable is 4.8915 greater than +1, therefore the sales variable is highly positively skewed. |

**Frequency distribution of all Categorical Variables**
The frequency distribution table of all the categorical variables are created to display the distinct values in the the dataset and the number of occurences (frequency counts) of each. Creating a frequency table makes it easier to view and understand the data at a glance. It gives the dataset a lot more meaning.

### GRAPHICAL UNIVARIATE ANALYSIS
Using plotly, histograms were plotted to show the frequency table of the following categories:
* Age_Group
* Customer_Gender
* Country
* State
* Product_Category
* Sub_Category
* Product
### INSERT ALL THE PHOTOS HERE


| Observation |
------------- |
| The conclusion below is based on the assumption that all orders are from unique customers. |
|  Most of the company's customers are adults, between the ages of 35 and 64. This is followed by the adults group (between the ages of 25 and 34. It means the sales and marketing team should focus most of their marketing efforts at this groups since thats where majority of their customers are. Another way to look at it is that, the company needs to come up with a marketing strategy to attract the older population 64 and above (if they want to get more of this age demographic). |
| Most of the company's customers are male. But then the number of female customers are not so far behind. |
| United states has the highest frequency of sale and Germany has the lowest. The reasons for this can then be further analyzed using more data from the company. |
| California stands out as the state with the highest frequency, followed by British Columbia. |
| The product_category with the highest frequency is Accesories. |
| The sub_category with highest frequency is Tires and tubes |
| Water bottle has the highest frequency | 


### Step 5: BIVARIATE ANALYSIS
Bivariate analysis is done using the target variable 'sales' and the different categorical variables. Firstly, it is done using the sum of sales and then it is done using the average sales (mean). Below are some of the graphs. 
# Add Graphs

### Step 6: Check the total sales by month and year and the average sales by month and year
Line Graps were plotted to answer the following questions:
* What is the average sale by month and year?
* What is the total sale by month and year?
## Add graphs

### Step 7: MULTIVARIATE ANALYSIS
The following visualizations were plotted for the multivariate analysis.
* Tree maps
* Correlation Matrix
* Heatmap






    
    

    

