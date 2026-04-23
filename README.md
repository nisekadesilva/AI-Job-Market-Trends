# AI Global Job Market Intelligence Dashboard
**Turning raw job postings into a story of opportunity, pay, and global workforce transformation**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0052CC?style=for-the-badge)
## <img src="https://cdn.simpleicons.org/readthedocs/4F46E5" width="20"/> | Project Overview 


 ### <img src="https://cdn.simpleicons.org/target/4F46E5" width="20"/> | Why This Project Matters

Artificial Intelligence is rapidly transforming the global job market.
But while everyone talks about AI replacing jobs, very few understand how the job market is actually evolving.

  -Which roles are growing? <br>
  -Who is earning the most? <br>
  -Is remote work really dominating?

This project answers those questions by turning raw job posting data into a clear, insight-driven story.

<b> Goal</b> - <i> Understand how salary, demand, and work structure are shaping AI careers globally.</i>


### <img src="https://cdn.simpleicons.org/duckduckgo/4F46E5" width="20"/> |  How I Approached This Problem

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

<b>Step 1 </b>| Data Validation ──────  <br>
  Checked for duplicate job entries → none affecting analysis <br>
  Verified missing values in key fields → no critical nulls found <br><br>
  
  
<b>Step 2 </b>| Standardization ────── <br>
  Renamed columns for clarity
  <i> Example: annual_salary_usd → Salary (USD) </i>
  Standardized categories (Remote, Hybrid, Onsite) <br><br>
  

<b>Step 3 </b>| Data Type Fixing  ────── <br>
  Salary → Decimal Number <br>
  Experience → Whole Number <br>
  Categories → Text <br><br>
  

<b>Step 4 </b>| Feature Preparation   ────── <br>
  Cleaned inconsistent labels  <br>
  Ensured uniform country and industry names<br><br>
  
  
<b>Step 5</b> | KPI Creation (DAX)   ────── <br>

<b>Total Jobs</b> → <code>COUNTROWS(AI_Jobs)</code><br>
<b>Avg Salary</b> → <code>AVERAGE(AI_Jobs[Salary])</code><br>
<b>Max Salary</b> → <code>MAX(AI_Jobs[Salary])</code><br>
<b>Remote Jobs</b> → <code>CALCULATE(COUNTROWS(AI_Jobs), AI_Jobs[Work Type] = "Remote")</code><br>
<b>Remote %</b> → <code>DIVIDE([Remote Jobs], [Total Jobs])</code> <br>


## <img src="https://cdn.simpleicons.org/chartdotjs/4F46E5" width="20"/> | Dashboard Story

The dashboard is designed as a 3-part analytical narrative

<b> 1. Market Overview </b> — Where are the opportunities?
   
<img width="1300" height="736" alt="Screenshot 2026-04-22 045822" src="https://github.com/user-attachments/assets/6189c97d-ca62-45f9-91d8-046fe3b00aed" />

Highlights <br>
──────
-Total AI job postings
-Maximum salary observed
-Remote job percentage
-Country-wise job distribution

Insight <br>
──────
<b> This section provides a global snapshot of AI job demand, highlighting both geographic distribution and how job postings evolve over time.<b> <br><br><br>
       ---- 1.Geographic Insight ---- <br><br><br>
       The distribution of job postings across countries shows a relatively balanced demand <br> <br>
          -The UK records the highest number of job postings (~8452) <br>
          -The USA shows the lowest (~8274)<br><br>
       However, the difference between countries is minimal, indicating that,<br>
       <b> <i> || AI job opportunities are globally distributed rather than concentrated in a single region. </b> </i><br><br><br><br>
       ---- 2.Time-based Insight ---- <br><br><br>
       Analyzing job postings over time reveals stable demand with slight fluctuations, <br><br>
           - 2024 shows the highest number of postings (~7312)<br>
           - 2023 records the lowest (~7035)<br>
           - Other years (2020–2026) remain within a similar range (~7100–7200)<br><br>
   <b> <i> || The AI job market is consistently active, without extreme spikes or drops. </b> </i>

               

<br> <br>

<b> 2. Salary Intelligence </b> — Who gets paid the most? 

<img width="1294" height="693" alt="Screenshot 2026-04-22 054905" src="https://github.com/user-attachments/assets/0c8615f8-2633-4ab8-8a3a-dab766f1c844" />

Highlights <br>
────── <br>
-Average salary by experience level<br>
-Salary by industry<br>
-Salary by job title<br>
-Salary by country<br>

Insight <br>
────── <br>
<b> Experience level plays a bigger role than location in determining salary<b> <br><br><br>

  ---- 1.Geographic Insight ---- <br><br><br>
       The distribution of job postings across countries shows a relatively balanced demand <br> <br>
          -The UK records the highest number of job postings (~8452) <br>
          -The USA shows the lowest (~8274)<br><br>
       However, the difference between countries is minimal, indicating that,<br>
       <b> <i> || AI job opportunities are globally distributed rather than concentrated in a single region. </b> </i><br><br><br><br>
       ---- 2.Time-based Insight ---- <br><br><br>
       Analyzing job postings over time reveals stable demand with slight fluctuations, <br><br>
           - 2024 shows the highest number of postings (~7312)<br>
           - 2023 records the lowest (~7035)<br>
           - Other years (2020–2026) remain within a similar range (~7100–7200)<br><br>
   <b> <i> || The AI job market is consistently active, without extreme spikes or drops. </b> </i>

<b>3. Job Market Structure </b> — How is the workforce evolving?

<img width="1116" height="591" alt="Screenshot 2026-04-22 045556" src="https://github.com/user-attachments/assets/8a23683e-7e12-4790-9ac5-fabb9273b887" />

Highlights<br>
────── <br>
-Industry demand <br>
-Work type distribution<br>
-Experience level distribution<br>


Insight <br>
──────<br>
<b>This section explores how AI jobs are distributed across work types and experience levels, revealing the structure of the modern AI workforce.<b><br><br><br>
       ---- 1.Work Type Distribution ---- <br><br><br>
       The distribution of work arrangements shows a highly balanced job market, <br> <br>
          - Hybrid roles: ~33.97% (~17,000 jobs) <br>
          - Remote roles: ~32.96% (~16,440 jobs) <br>
          - Onsite roles: ~33.8% (~16,580 jobs)<br><br>
       While hybrid roles appear slightly higher, the differences are marginal, indicating that,<br>
       <b> <i> || The AI job market is evenly split across remote, hybrid, and onsite models, rather than being dominated by remote work. </b> </i><br><br><br><br>
       ---- 2.Experience Level Distribution ---- <br><br><br>
      The distribution of jobs across experience levels shows a slight concentration in mid-level roles, <br><br>
           - Mid-level roles: ~16,720 jobs<br>
           - Entry-level roles: ~16,620 jobs <br><br>
      Although mid-level roles have the highest count, the difference is very small (~100 jobs), suggesting that<br>
   <b> <i> || Demand is relatively balanced across experience levels, with a slight preference for candidates with some experience. </b> </i>

## <img src="https://cdn.simpleicons.org/grafana/4F46E5" width="20"/> | Tools & Technologies
-Power BI <br>
-DAX (Data Analysis Expressions)<br>
-Power Query<br>
-Data Modeling<br>
-Data Visualization<br>

<img src="https://cdn.simpleicons.org/toolbox/4F46E5" width="20"/> 
<img src="https://cdn.simpleicons.org/databricks/4F46E5" width="20"/> Key Insights
<img src="https://cdn.simpleicons.org/grafana/4F46E5" width="20"/> Dashboard


