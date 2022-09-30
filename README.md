# Sales Exploratory Data Analysis with Python

#### OBJECTIVE
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

#### TOOLS
The main tool used for this project is **Python**. The following Python Libraries are used for the project:
> * **Pandas**
> * **NumPy**
> * **Matplotlib**
> * **Seaborn**
> * **Plotly**
> * **wordCloud**


#### PROCEDURE
The project is broken down into the following steps:

1.  **Overview and summary of the data:** 
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
 > **Conclusion:**
    * There were no missing values in the sales data set.
    * The dataset had 13 columns
    * The dataset had 113035 rows of data
    * The date column was not in the correct datatype 'datetime'
   
  
 2. **Data Cleaning and Preparation**
    The data did not need much cleaning. However, some new columns had to be created
    * Conversion of date column from object to datetime
    * Extraction of the Year, Month and Day from the Date column and creating new columns for them
    * Calculation of Total sales and Profit and creating 2 new columns for the results
  
  3. **Checking the unique values in each column to answer the following questions:
    * What is the customer demographic, in terms of age?
    * What countries and states do the company serve?
    * What products do the company sell?
    * How are the products categorised?
   
  4. **Univariate Analysis**
  
       **Non-Graphical Univariate Analysis:**
 **Measure of Central Tendency and Dispersion**
The first type of univariate analysis conducted was the non-graphical univariate analysis.
Since the company's major focus was on sales, the target variable in the analysis is 'Sales' variable. The Central tendency and dispersion of the sales variable is checked. Central tendency is a statistical measure which identifies a single value as representation of an entire distribution. The mean is the most common central tendency and for this sales variable, the mean is used as the central tendency. Dispersion shows the distribution or spread of the data and the most common measures of dispersion are standard deviation, variance and interquartile range. 
   * Using the **describe() method, the central tendency and dispersion are given.**
  
  **Measure of Skewness**
  The statistical measures that show the shape of the distribution of the data are skewness and kurtosis. Skewness is a measure of asymetry: it defines the extent to which a distribution differs from normal distribution. A distribution may have a right(positive) skewness or a left(negative) skewness or zero skewness. 
  * Positive skewness means the data is skewed to the right, the data is concentrated to the right and the value is poitive. mean > median > mode.
  * Negative skewness means the data is skewed to the left, the data concentration is on the left and the value is negative. mean < median < mode.
  * Zero skewness means the data is symmetrical and the distibution is normal. It is depicted by zero. mean = median = mode
  * Skewness between -0.5 and 0.5 means the data is fairly symmetrical.
  * Skewness between -1 and 0.5 means the data is moderately skewed.
  * Skewness less than -1 or greater than 1 means the data is highly skewed.
  * Using the .skew() function, the distribution of the data is given, in terms of skewness
   
  > **Conclusion**
  * The minimum sales value is 2, the maximum sales value is 69136 and the count is 113036.
  * The measure of dispersion(standard deviation) is 1466.202934.
  * The central tendency given by the mean is 842 and given by the median is 245.
  * IQR is the difference between the 75th and 25th percentile, and the IQR for the sales variable is 810
  * The skewness of the sales variable is 4.8915 greater than +1, therefore the sales variable is highly positively skewed.

**FREQUENCY DISTRIBUTION OF CATEGORICAL VARIABLES**
The frequency distribution of all the categorical variables is created to show the distinct values in the the dataset and the number of occurences (frequency counts) of each. It makes it easier to view and understand the data at a glance.


    
    

    

