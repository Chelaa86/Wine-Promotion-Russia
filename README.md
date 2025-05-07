# Excel Dashboard Report

## Project Overview
### Background
Your company owns a chain of stores across Russia that sell a variety of alcoholic drinks. The company recently ran a wine promotion in Saint Petersburg that was very successful. Due to the cost to the business, it isn’t possible to run the promotion in all regions. The marketing team would like to target 10 other regions that have similar buying habits to Saint Petersburg where they would expect the promotion to be similarly successful.

## Data Sources
The marketing team has sourced you with historical sales volumes per capita for several different drinks types.
 - "year": year (1998-2016)
 - "region": name of a federal subject of Russia. It could be oblast, republic, krai, autonomous okrug, federal city and a single autonomous oblast
 - "wine": sale of wine in litres by year per capita
 - "beer": sale of beer in litres by year per capita
 - "vodka": sale of vodka in litres by year per capita
 - "champagne": sale of champagne in litres by year per capita
 - "brandy": sale of brandy in litres by year per capita

## Tool Used
MS Excel

## Data Cleaning
- Converted the dataset into a table for easier manipulation and analysis.
- Worked with the "year", "region", "wine" columns since we're focusing on wine promotion.
- Data formatting e.g. ensuring "region" column is text.
- Checked for duplicates; didn't find any duplicates.
- Checked for missing values;
    - removed **Chechen Republic** since it had blanks in the wine column from 1998-2016.
    - replaced the remaining blanks with mean wine consumption per year.  

## Exploratory Data Analysis(EDA)




