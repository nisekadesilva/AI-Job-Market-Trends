# AI Global Job Market Intelligence Dashboard
**Turning raw job postings into a story of opportunity, pay, and global workforce transformation**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0052CC?style=for-the-badge)

## Why This Project Matters

Artificial Intelligence is rapidly transforming the global job market.
But while everyone talks about AI replacing jobs, very few understand how the job market is actually evolving.

  -Which roles are growing? <br>
  -Who is earning the most? <br>
  -Is remote work really dominating?

This project answers those questions by turning raw job posting data into a clear, insight-driven story.

<b> Goal</b> - <i> Understand how salary, demand, and work structure are shaping AI careers globally.</i>


## <img src="https://cdn.simpleicons.org/duckduckgo/4F46E5" width="20"/> | ## How I Approached This Problem

Instead of jumping straight into charts, I followed a structured data analysis workflow:

  -Explored and understood the dataset <br>
  -Validated data quality (duplicates, missing values) <br>
  -Cleaned and standardized the data <br>
  -Built analytical KPIs using DAX <br>
  -Designed a dashboard focused on storytelling
   
## <img src="https://cdn.simpleicons.org/chartdotjs/4F46E5" width="20"/> |  Dataset Information

Source -  Kaggle / Public AI Job Market Dataset <br>
Type - Real-world scraped job postings dataset <br>
Size - Large-scale dataset (~thousands of records)


Fields Included 
──────────────

<ul> 
<li>Job Title</li>
<li>Company Type (Startup / MNC / Research Lab)</li>
<li>Industry Sector</li> 
<li>Country</li>
<li>Work Type (Remote / Hybrid / Onsite)</li>
<li>Experience Level</li>
<li>Years of Experience</li>
<li>Job Posted Year </li>
<li>Annual maximun Salary (USD)</li> </ul> 

## <img src="https://cdn.simpleicons.org/redux/4F46E5" width="20"/> | Data Preparation

Data preparation was treated as a data quality investigation process:

Step 1 | Data Validation ──────  <br>
  Checked for duplicate job entries → none affecting analysis
  Verified missing values in key fields → no critical nulls found
  
Step 2 | Standardization ────── <br>
  Renamed columns for clarity
  <i> Example: annual_salary_usd → Salary (USD) </i>
  Standardized categories (Remote, Hybrid, Onsite) 

Step 3 | Data Type Fixing  ────── <br>
  Salary → Decimal Number <br>
  Experience → Whole Number <br>
  Categories → Text <br>

Step 4 | Feature Preparation   ────── <br>
  Cleaned inconsistent labels  <br>
  Ensured uniform country and industry names
  
Step 5 | KPI Creation (DAX)   ────── <br>

   Total Jobs = COUNTROWS(AI_Jobs)

   Avg Salary = AVERAGE(AI_Jobs[Salary])

   Max Salary = MAX(AI_Jobs[Salary])

   Remote Jobs = 
   CALCULATE(COUNTROWS(AI_Jobs), AI_Jobs[Work Type] = "Remote")

   Remote % = 
   DIVIDE([Remote Jobs], [Total Jobs])

<b>Total Jobs</b> → <code>COUNTROWS(AI_Jobs)</code><br>
<b>Avg Salary</b> → <code>AVERAGE(AI_Jobs[Salary])</code><br>
<b>Max Salary</b> → <code>MAX(AI_Jobs[Salary])</code><br>
<b>Remote Jobs</b> → <code>CALCULATE(COUNTROWS(AI_Jobs), AI_Jobs[Work Type] = "Remote")</code><br>
<b>Remote %</b> → <code>DIVIDE([Remote Jobs], [Total Jobs])</code>

## | Dashboard Story

The dashboard is designed as a 3-part analytical narrative



1. Market Overview — Where are the opportunities?

👉 (Insert Overview page screenshot here)

![Overview](screenshots/overview.png)
Highlights
──────
-Total AI job postings
-Maximum salary observed
-Remote job percentage
-Country-wise job distribution

💡 Insight:
Gives a global snapshot of AI job demand and scale

🟩 2. Salary Intelligence — Who gets paid the most?

👉 (Insert Salary page screenshot here)

![Salary Analysis](screenshots/salary.png)
Highlights:
Average salary by experience level
Salary by industry
Salary by job title
Salary by country

💡 Insight:
Experience level plays a bigger role than location in determining salary

🟨 3. Job Market Structure — How is the workforce evolving?

👉 (Insert Insights page screenshot here)

![Job Market Insights](screenshots/insights.png)
Highlights:
Industry demand
Work type distribution
Experience level distribution

📌 Key Finding:

Remote: 32.96% (~16K jobs)
Hybrid: 33.97% (~17K jobs)
Onsite: 33.8% (~17K jobs)

💡 Insight:
Remote work is important — but not dominant


<img src="https://cdn.simpleicons.org/toolbox/4F46E5" width="20"/> 
<img src="https://cdn.simpleicons.org/databricks/4F46E5" width="20"/> Key Insights


