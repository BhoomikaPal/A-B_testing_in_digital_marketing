# A/B_testing_in_digital_marketing
A/B testing is a technique often used by marketing companies to evaluate the performance of different campaign strategies. It involves showing different versions of a variable (such as an advertisement or web page) to separate audience segments simultaneously, in order to determine which version has the greatest impact.

In this project, we analyze the results of an A/B test where the **experimental group** is shown ads, while the **control group** sees either a Public Service Announcement (PSA) or nothing at all. Our goal is to answer the following key questions:

- **Is the marketing campaign effective?**
- **How much of the success can be attributed to the ads?**

## Objectives
- Compare performance between control and experimental groups  
- Measure the effectiveness of digital ads  
- Determine if the observed differences are **statistically significant**

## Dataset Overview:
-  **converted_int:** Whether the user converted (1 = yes, 0 = no)
-  **total ads:** Total number of ads seen
-  **test group:** Whether the user saw an actual ad or a Public Service Announcement (PSA)
-  **most ads day:** Day of the week with highest ad exposure for the user

## Approach
We perform the following steps using Python:

1. **Exploratory Data Analysis (EDA)**  
   - Understand data structure  
   - Visualize group-wise performance metrics  

2. **Hypothesis Testing** - We created a robust testing function using:
  - **Shapiro-Wilk Test** for normality
  - **Levene's Test** for variance homogeneity
  - **Mann-Whitney U Test** (non-parametric alternative)

## Tools & Technologies

- Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn)
- Google Colaboratory

## Key Insights:
  - Users who converted saw significantly more ads than those who didn’t
  - Weekdays had higher ad exposure compared to weekends
  - The 'ad' group saw more ads on average than the 'PSA' group

Original data Source: Kaggle Marketing A/B Testing Data

