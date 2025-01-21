
# Pharmaceutical Market Analysis
## Problem Statement:
Dr. Malhotra's Laboratories Pvt. Ltd. plans to enter the Bangladeshi generic medicine market. The predictions indicate that there is going to be a lot of cases of malaria and dengue. Focus on antimalarial and anti-pyretic (fever reducing) drug classes and perform market landscape analysis for these sub-segment...

## Overview
The Pharma Market Analysis Dashboard is an interactive tool designed to provide insights into the pharmaceutical market. It consolidates key data points such as medicine brands, manufacturers, drug classes, generics, and dosage forms to aid stakeholders in making informed decisions.

## About the DataSet:
This dataset has 6 CSV files elaborating the details of Bangladesh Generic Medicine market. Data was scraped from the medex sub-domain of Bangladesh.

| Filename | Information about |
| ------------- | ------------- |
| medicine.csv | Generic medicines available in the Bangladesh Generic Medicine market.  |
| manufacturer.csv  | Manufacturers of generic medicines in the Bangladesh Generic Medicine market.  |
|indication.csv|Medical indications, which are the specific conditions or diseases for which generic medicines are prescribed.|
|generic.csv|Generic drugs, including their characteristics and usage details.|
|drug class.csv|Drug classes, which categorize generic medicines based on their therapeutic classes or categories.|
|dosage form.csv|The various dosage forms in which generic medicines are available.|
|Column_Description.xlsx|The columns of all tables in the dataset. (No need to load this file into your visualization tool, it is just for understanding the dataset.)|

## Objectives
- Understand the market size and growth trends in Bangladesh
- Identify key players and their market share
- Analyze regulatory influences
- Evaluate emerging trends and innovations
- Assess the competitive landscape

## Exploratory Data Analysis Questions:

1.  How many medicine brands, generics, manufacturers, drug classes and dosage forms (approximate value) are available in Bangladesh Generic Medicine Market?

2.  What is the percentage of herbal medicine available in Bangladesh?

3.  What is the most available dosage form?

4.  Which generic has the highest associated number of medicines?

5.  What is the top drug class in terms of the number of generics?

6.  Which pharmaceutical company has the highest number of medicines?

7.  What is the association (type of relationship) between drug classes and generics?

8.  What is the correlation between competitiveness and average price (averaged across dosage form per combination of manufacturer and generic)?
9.  Does dosage size have the same unit?
## Questions Related to Problem Statement:
1.  For antimalarial drugs, how many competitors(manufacturers and Brands) are there in this market?

2.  Are there any generic drug formulas in the anti-malarial drug class with a single competitor?

3.  Suggest an entry price for an anti-malarial (Mefloquine) drug to stay competitive given that the dosage size is the same as that of the competitor.

4.  How many Paracetamol (IV Infusion) suppliers are there?

5.  What is the number of competitors(manufacturers) for insulin drugs (include all subcategories with the word insulin)?

6.  Compared to insulin, does the anti-hypertensive drug segment have more competitors(manufacturers and brands)? [include all subcategories with the word anti-hypertensive]
### Steps Followed:
-  Step 1: Loaded datasets into Power BI.
-  Step 2: Reviewed the column profiles of all datasets.
-  Step 3: Removed the slug column from all datasets.
-  Step 4: Transformed medicine.csv by splitting the package container column to extract price details.
-  Step 5: Analyzed dataset columns and established the ER model. Link to
        <a href= "https://github.com/raju-payyavula/Pharmaceutical-Market-Analysis/blob/main/ER%20Model.PNG"> ER Model </a>
-  Step 6: Created a measure to calculate average generic prices using the formula: Avg Price = AVERAGE(medicine[price]).



