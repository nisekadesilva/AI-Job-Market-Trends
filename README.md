# AI Global Job Market Intelligence Dashboard
**Turning raw job postings into a story of opportunity, pay, and global workforce transformation**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0052CC?style=for-the-badge)

# Why This Project Matters

Artificial Intelligence is rapidly transforming the global job market.
But while everyone talks about AI replacing jobs, very few understand how the job market is actually evolving.

  -Which roles are growing?
  -Who is earning the most?
  -Is remote work really dominating?

This project answers those questions by turning raw job posting data into a clear, insight-driven story.

<b> Goal</b> - <i> Understand how salary, demand, and work structure are shaping AI careers globally.</i>

# How I Approached This Problem

Instead of jumping straight into charts, I followed a structured data analysis workflow:

  -Explored and understood the dataset
  -Validated data quality (duplicates, missing values)
  -Cleaned and standardized the data
  -Built analytical KPIs using DAX
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

Step 1 | Data Validation ──────────────
  Checked for duplicate job entries → none affecting analysis
  Verified missing values in key fields → no critical nulls found
  
Step 2 | Standardization ──────────────
  Renamed columns for clarity
  <i> Example: annual_salary_usd → Salary (USD) </i>
  Standardized categories (Remote, Hybrid, Onsite) 

Step 3 | Data Type Fixing
  Salary → Decimal Number
  Experience → Whole Number
  Categories → Text

Step 4 | Feature Preparation
  Cleaned inconsistent labels
  Ensured uniform country and industry names
  
Step 5 | KPI Creation (DAX)

Total Jobs = COUNTROWS(AI


## <img src="https://cdn.simpleicons.org/duckduckgo/4F46E5" width="20"/> | What I explored

- Where are AI jobs most in demand globally?
- What factors influence salary the most?
- Which industries are hiring the most AI talent?
- How is remote work distributed globally?
- What experience level dominates high-paying roles?


<img src="https://cdn.simpleicons.org/toolbox/4F46E5" width="20"/> 


