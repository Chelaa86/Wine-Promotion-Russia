# Excel Dashboard Report
## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tool Used](#tool-used)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

## Project Overview
### Background
Your company owns a chain of stores across Russia that sell a variety of alcoholic drinks. The company recently ran a wine promotion in Saint Petersburg that was very successful. Due to the cost to the business, it isn’t possible to run the promotion in all regions. The marketing team would like to target 10 other regions that have similar buying habits to Saint Petersburg where they would expect the promotion to be similarly successful.
![Excel_2](https://github.com/user-attachments/assets/bcddde8f-b03b-4e03-bc5c-54eb24882844)
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

## Exploratory Data Analysis
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

## Data Analysis
**Method Used: Correlation Analysis**

Used Pearson correlation to measure the strength of linear association between wine sales in **Saint Petersburg** and wine sales in other regions over the years 1998–2016.

### Findings
- Identified the **Top 10 regions** with the highest positive correlation to Saint Petersburg’s wine consumption trends.
- These regions are potential targets for future promotions, as they exhibit similar consumer behavior patterns.

### Insights
- High-correlation regions demonstrated not only similar yearly trends but also responded similarly to economic and social changes over time.
- This makes them strong candidates for campaign replication.

## Recommendations
1. **Target the Top 10 High-Correlation Regions**

Focus future wine promotions on the regions that demonstrated the strongest positive correlation with Saint Petersburg's wine consumption patterns. These regions are likely to respond similarly to marketing efforts.

2. **Pilot the Campaign in 2–3 High-Potential Regions First**

Before a full rollout, run smaller promotions in 2–3 of the top-ranked regions to validate assumptions and gather real-time performance data.

3. **Incorporate Multi-Product Analysis in Future Work**

Expand future analyses to include beer, vodka, champagne, and brandy to identify cross-category promotional opportunities and understand broader alcohol consumption trends.

4. **Consider Socioeconomic and Demographic Factors**

Supplement consumption data with income levels, population size, or cultural preferences per region to better tailor marketing strategies.

5. **Monitor and Measure Promotion Outcomes**

After running the promotions, track performance metrics such as sales lift, customer engagement, and ROI to validate the strategy and improve future targeting.

## Limitations
**Single-Variable Focus (Wine Only)**

The analysis was based solely on the "wine" column, excluding other alcoholic beverages such as beer, vodka, champagne, and brandy. This narrow focus may not fully capture regional preferences for alcohol consumption, which could influence the effectiveness of cross-product promotions.

**Exclusion of the Chechen Republic**

The Chechen Republic was removed from the analysis due to missing wine consumption data for all years. While necessary for data quality, this may have excluded a region with unique or valuable consumption patterns across other drink categories.

**Assumption of Correlation = Suitability**

High correlation in wine consumption trends does not guarantee a promotion’s success. Other factors — such as demographics, income levels, and cultural preferences — were not considered but could impact campaign outcomes.

**No Consideration for Seasonal or Promotional Effects**

The data did not explicitly account for temporary promotions, holidays, or events that may have influenced year-over-year wine sales, potentially skewing the correlation.

**Static Time Window (1998–2016)**

The analysis was limited to historical data ending in 2016. Current consumption patterns may have shifted, and the findings may not reflect recent behavioral changes or market dynamics.

## References

This project was completed as part of the *Her Data Project*, a program designed to empower fellows in data analytics through practical, real-world projects and mentorship.
