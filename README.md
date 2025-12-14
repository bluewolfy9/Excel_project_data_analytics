# Excel_project_data_analytics

Key Questions Explored

I analyzed the dataset to answer the following critical questions:

    Do more skills translate to better pay?

    What is the salary outlook for data jobs across different regions?

    What are the most requested skills for data professionals?

    What is the median pay associated with the top 10 skills?

🛠️ Core Excel Analysis Toolkit

This analysis was built entirely within Excel, utilizing the following advanced features:

    📊 Pivot Tables & 📈 Pivot Charts: For summarizing data and visualizing insights.

    🧮 DAX (Data Analysis Expressions): Used for advanced calculations like median salary.

    🔍 Power Query: Essential for data extraction, transformation, and cleaning (ETL).

    💪 Power Pivot: Used to create a powerful Data Model for integrated analysis.

🗃️ Data Jobs Dataset

The dataset contains real-world data science job information from 2023, sourced from my Excel course. It provides detailed information on:

    👨‍💼 Job titles

    💰 Salaries

    📍 Locations

    🛠️ Skills

1️⃣ Do More Skills Get You Better Pay?
🔍 Power Query (ETL) Process

    📥 Extract: The original data (data_salary_all.xlsx) was imported via Power Query, creating two foundational queries: one for all job information (data_jobs_all) and a second listing skills per job ID (data_job_skills).

    🔄 Transform: Both queries were cleaned by modifying column types, removing unnecessary fields, eliminating specific text, and trimming whitespace.

    🔗 Load: The two transformed queries were loaded into the workbook, ready for analysis.

📊 Analysis & Insights

    💡 Insights: There is a positive correlation between the number of requested skills and the median salary, especially for roles like Senior Data Engineer and Data Scientist.

        Roles demanding fewer skills (e.g., Business Analyst) tend to have lower salaries, indicating that specialized, multi-faceted skill sets command higher market value.

    🤔 So What: This emphasizes that investing in acquiring multiple relevant skills is crucial for professionals aiming for top-tier, higher-paying roles.

2️⃣ What’s the Salary for Data Jobs in Different Regions?
🧮 PivotTables & DAX

A PivotTable was used to summarize salary data by job title and region, with DAX measures created to calculate the median salary.

    DAX Formula Example (US Median Salary):
    =CALCULATE(MEDIAN(data_jobs_all[salary_year_avg]),data_jobs_all[job_country]="United States")

    The overall median salary was calculated using: Median Salary:=MEDIAN(data_jobs_all[salary_year_avg]).

📊 Analysis & Insights

    💡 Insights: High-level roles like Senior Data Engineer and Data Scientist command higher median salaries globally, confirming their high demand.

        A notable salary disparity exists between US and Non-US roles in high-tech positions, likely due to the concentration of major tech industries in the US.

    🤔 So What: These geographical salary insights are essential for negotiation and strategic career planning, ensuring compensation aligns with global and regional market standards.

3️⃣ What are the Top Skills of Data Professionals?
🔧 Power Pivot for Data Modeling

    💪 Data Model: The data_jobs_all and data_job_skills tables were integrated using Power Pivot, creating a relationship based on the common job_id column.

    🔗 Relationship: The pre-cleaned data (from Power Query) allowed for an easy, seamless relationship creation within the Power Pivot menu.

📊 Analysis & Insights

    💡 Insights: SQL and Python are the dominant, foundational skills requested in data-related jobs.

        A significant presence of emerging technologies like AWS and Azure highlights the industry's strong shift towards cloud services and big data infrastructure.

    🤔 So What: Understanding these prevalent skills guides professionals on where to focus their learning to stay competitive and maximize their career impact.

4️⃣ What’s the Pay of the Top 10 Skills?
📊 Advanced Charts (PivotChart)

A combo PivotChart was created from the final PivotTable to simultaneously visualize two metrics:

    🪙 Primary Axis: Median Salary (as a Clustered Column)

    👍 Secondary Axis: Skill Likelihood (as a Line with Markers)

📊 Analysis & Insights

    💡 Insights: Skills like Python, Oracle, and SQL are associated with the highest median salaries, confirming their critical role in high-paying tech sectors.

        Conversely, generic skills like PowerPoint and Word showed the lowest median salaries and likelihood, reflecting lower specialization demand in high-salary roles.

    🤔 So What: This visualization strongly reinforces the importance of investing in high-value, specialized skills like Python and SQL for maximizing salary potential in the tech industry.

💡 Conclusion

This was a successful Excel-based project in translating real-world job posting data into actionable career intelligence through the leverage of Power Query, PivotTables, DAX, and Power Pivot. Key correlations have been established between the number of skills and higher salaries, with Python, SQL, and cloud technologies identified as essential for top pay.
It gives data professionals a realistic, data-driven roadmap on which skills to acquire to reach higher-paying roles.
