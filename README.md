# Introduction
This project analyzes the Wine.csv dataset using exploratory data analysis (EDA) to uncover patterns and insights into the most reviewed wines, quality ratings, and other key factors using Python. The analysis includes data preprocessing, visualization, and statistical summaries to better understand the attributes influencing wine quality.

### Summary of the data set
The dataset used for this analysis provides detailed information about a wide variety of wines from across the globe. It includes the following columns:
1.	Unnamed:0: A numerical index column that uniquely identifies each record.
2.	Country: The country where the wine was produced.
3.	Description: A textual description of the wine, often highlighting its taste, aroma, and other notable qualities.
4.	Designation: The specific vineyard or wine label associated with the wine.
5.	Points: A rating score for the wine, typically out of 100, provided by experts.
6.	Price: The price of the wine in USD.
7.	Province: The province or state where the wine was produced.
8.	Region_1: A more localized region within the province or state of production.
9.	Region_2: A smaller area within the region that gives more detailed location information (though some data might be missing).
10.	Variety: The grape variety used to produce the wine (e.g., Chardonnay, Merlot).
11.	Winery: The name of the winery that produced the wine.
The dataset is suitable for a wide range of analyses, including evaluating the relationships between wine ratings, prices, and regional characteristics, as well as identifying trends in wine preferences by variety or country. It also allows for textual analysis of descriptions to uncover common terms used in wine reviews.
The analysis of this dataset revealed insights into wine quality, pricing patterns, and geographical influences, providing a comprehensive understanding of the factors that make a wine stand out.

### DATA CLEANING
The data cleaning process involved a combination of tools, libraries, and visualizations to prepare the dataset for analysis. The following tools and libraries were utilized:
1.	Python: Used for executing all data cleaning tasks.
2.	Pandas: Essential for data manipulation, handling missing values, and cleaning the dataset.
3.	NumPy: Used for mathematical operations and array handling during the cleaning process.
4.	Jupyter Notebooks: Provided an interactive environment for code development, exploration, and documentation.
5.	Plotly: Enabled interactive data visualizations to communicate findings effectively.
The dataset was thoroughly examined to understand its structure, columns, and meanings. Exploratory Data Analysis (EDA) was conducted to gain insights, identify patterns, and uncover anomalies.

#### Key Data Cleaning Steps:
•	The Unnamed: 0 column was dropped as it contained no meaningful information.
•	Missing values were addressed by using the .fillna() function for certain columns, while columns with a significant percentage of missing values, such as region_2, were removed.
Visualizations for Data Understanding and Cleaning:
•	A scatter plot was created to examine the relationship between wine quality (points) and price, revealing any trends or correlations.
•	Bar charts highlighted the most reviewed wine varieties and the countries producing the most expensive wines, providing insights into consumer preferences and industry trends.
•	A histogram was used to visualize the distribution of wine quality ratings (points), helping identify patterns or anomalies in the rating scale.
These tools, methods, and visualizations worked together to ensure the dataset was clean, well-understood, and ready for further analysis. The process not only prepared the data but also uncovered valuable insights about wine quality, pricing, and regional production trends.

### MISSING DATA
The missing values in the dataset were identified as NaN in the columns designation, region_1, and region_2. To handle these missing values, the .fillna() function was applied to the designation and region_1 columns. For these columns, appropriate default values were used to replace the NaN entries, ensuring no data was left unaccounted for. The region_2 column, on the other hand, had more than 50% of its values missing. Due to the significant amount of missing data, this column was dropped using the .drop() method, as retaining it could have compromised the integrity of the analysis. These approaches ensured the dataset remained clean and usable for further analysis.

### DATA STORIES AND VISUALISATIONS
The visualizations reveal several stories and insights about the dataset:
1.	#### Relationship Between Price and Quality (Scatter Plot)
2.	![Wine Scatter plot](https://github.com/user-attachments/assets/d60f78b4-af43-44b5-9804-53a21bce93ac)


The scatter plot exploring the relationship between wine price and quality (points) shows a general trend where higher-priced wines tend to score higher ratings. However, the relationship is not perfectly linear, as some lower-priced wines achieve high scores, suggesting that price is not the sole determinant of quality. This could point to the presence of high-value wines in affordable ranges.
2.	#### Most Reviewed or Rated Varieties (Bar Chart)
![Wine bar plot 2](https://github.com/user-attachments/assets/7f91e140-9f6f-4759-9b5c-91add09b5fbe)


The bar chart displaying the most reviewed wine varieties highlights consumer preferences. Varieties like Pinot Noir and Chardonnary dominate the dataset, reflecting their popularity or accessibility in the market. This could indicate consumer bias toward certain types of wine or an industry focus on these varieties.
3.	#### Countries Producing the Most Expensive Wines (Bar Chart)
![Bar plot 3](https://github.com/user-attachments/assets/ef774afa-f7a4-4ba2-9d80-af6c2346d779)


The bar chart comparing wine prices by country identifies regions with a reputation for premium wines. Countries such as New Zealand and Italy consistently produce higher-priced wines, suggesting they are known for luxury or exclusive wine markets. Conversely, countries with lower average wine prices might cater to more budget-friendly markets.
4.	#### Distribution of Quality Ratings (Histogram)
![4th pic](https://github.com/user-attachments/assets/4db8978b-f9f1-4331-80de-f77e71ecead2)


The histogram of wine quality ratings (points) reveals a clustering of ratings within a certain range, such as 85–95 points. This indicates that most wines meet a specific quality standard, with few outliers achieving exceptionally high or low scores. The lack of wines with extremely low scores might reflect a focus on including only marketable products in the dataset.

### Assumptions:
•	Higher-priced wines are often associated with better quality, but there are exceptions where affordable wines are highly rated.
•	Consumer preferences for certain wine varieties influence the number of reviews, potentially driving demand for those varieties.
•	Countries producing expensive wines might focus on premium production or have strong reputations in the global wine market.
•	The dataset might exclude low-quality wines, focusing more on wines that meet certain minimum market standards.

### Installation & Setup 🚀
To set up the project on your local machine:
- Clone the repository and navigate into the project directory.
- Create a virtual environment (recommended for dependency management).
- Install the required dependencies listed in requirements.txt.
- Launch Jupyter Notebook if working with Capstone_project.ipynb files.
  
### Usage 📊
After completing the setup, you can:
- Open Jupyter Notebook and run the analysis step by step.
- Modify and explore different dataset parameters.
- Generate visualizations to uncover insights related to car prices, fuel efficiency, and consumer behavior.
- Run Python scripts to analyze trends and patterns in the wine dataset.
  
THIS REPORT WAS WRITTEN BY : DAVID SETHATHI
