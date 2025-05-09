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
**1. Trend analysis for Saint Petersburg**.
- Purpose: Since the wine promotion was successful in **Saint Petersburg**, it was essential to understand its wine consumption behavior over time.
- Action: A line plot was created showing per capita wine consumption in **Saint Petersburg** from 1998 to 2016.
- Insights Gained: This helped in identifying if consumption was stable, increasing, or fluctuating, which would influence how "similar" other regions should be to it.
- Why it matters: If **Saint Petersburg** has a consistent or upward trend, we would want to find regions with similar long-term patterns.

**2. Regional wine consumption overview**.
- Purpose: To get a snapshot of which regions generally consume more or less wine on average.
- Action: The mean per capita wine consumption was calculated for each region across all available years.
- Visualization: A ranked table was used to compare regions based on these averages.
- Insights Gained: This showed which regions might be candidates for the promotion at a high level, before deeper analysis.

**3. Identified outliers**.
- Purpose: Outliers can distort analysis.
- Action: Used box plot to detect regions with irregular consumption (e.g., sudden spikes/drops).
- Insights Gained: Identified any regions with abnormal behavior that may not be suitable for comparison with **Saint Petersburg**.

**4. Standardized consumption values**.
- Purpose: Since different regions have different base levels of consumption, standardizing (e.g., using z-scores) helps compare them fairly.
- Action: Transformed the wine consumption data so each region’s values could be compared on a similar scale.
- Why it matters: This prepared the data for similarity analysis by reducing bias due to raw scale differences.

