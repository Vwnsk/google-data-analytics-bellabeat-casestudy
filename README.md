# google-data-analytics-bellabeat-casestudy
Case Study Bellabeat - Conclusion Project Google Data Analytics

The 6 Phases of the Data Analysis Process
This project followed the six phases of the data analysis process to ensure a structured approach, from defining the business problem to delivering strategic recommendations.

1. Ask Phase
The project began with a clear business task requested by Bellabeat's leadership: to analyze smart fitness device usage data to identify trends and, based on them, propose new marketing strategies to drive company growth. The primary objective was to turn raw data into actionable business insights.

2. Prepare Phase
In this phase, a public dataset from Kaggle (Fitbit Fitness Tracker Data) containing data from 33 users was used. Preparation involved a critical analysis of the data source, where its main strengths (data granularity) and weaknesses, such as the limited sample size and the fact that the data is from 2016, were identified. This initial assessment was crucial for contextualizing future findings.

3. Process Phase
This was the most technically challenging phase. The data was uploaded to Google BigQuery for processing with SQL. I faced and solved several import issues, including inconsistencies in CSV file delimiters (some used commas, others semicolons) and data type detection errors. The solution involved manually defining the table schemas, ensuring the integrity and proper structuring of the data for analysis. I also performed data cleaning and formatting on the date columns, converting them from STRING to TIMESTAMP to enable time-series analysis.

4. Analyze Phase
With the data cleaned, the analysis focused on discovering behavioral patterns. The first major finding was that users spent, on average, more than 16 hours a day in a sedentary state. I investigated the hypothesis that this was a measurement error (e.g., users not wearing the device 24/7), but the data proved that the usage time was for the full day. Deepening the analysis with a JOIN between activity and sleep data, I uncovered the main insight: even after subtracting the ~7 hours of sleep, there were still almost 5 hours of inactivity during the waking day. Furthermore, I confirmed a strong positive correlation between total steps and calories burned.

5. Share Phase
To communicate the findings effectively, I connected BigQuery to Looker Studio and created a visual dashboard. The visualizations included:

Scorecards to highlight the average distribution of minutes by activity type.

A Scatter Plot to illustrate the relationship between steps and calories.

A Comparative Bar Chart to show the difference between sleep time and awake sedentary time.
These visuals were essential for telling the data's story in a clear and impactful way.

6. Act Phase
The final phase consisted of translating the insights into business strategy. Based on the findings, I developed three strategic recommendations for Bellabeat:

"Active Wellness Journey": A feature in the app to combat daily sedentary time with smart notifications.

"Premium Sleep Assistant": An evolution of the sleep feature to drive the subscription service.

"Bellabeat Community": An engagement platform to educate on features and strengthen the brand.

Each recommendation was directly supported by data and focused on generating value for both the user and the company.
