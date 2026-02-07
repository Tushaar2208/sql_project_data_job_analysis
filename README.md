# 📊 Data Analyst Job Market Analysis

**Based on the dataset from [Luke Barousse's SQL Course](https://lukebarousse.com/sql).**

📂 **SQL queries? Check them out here:** [**project_sql folder**](/project_sql/)

## Introduction
This project explores the data analyst job market, focusing on the most well-paid and in-demand skills.
**The Goal:** To identify the optimal skills for data analysts to learn to maximize their salary potential and marketability.

**SQL queries** were used to inspect a dataset of job postings (`job_postings_fact`) to answer specific questions about the data field.

## Background
Using a dataset of job postings, I analyzed key metrics such as average salaries, skill demand, and company insights. The data was cleaned and validated to ensure accurate reporting.

### The Questions
The analysis is broken down into the following SQL queries:
1.  **What are the top-paying data analyst jobs?** ([`1_top_paying_jobs.sql`](project_sql/1_top_paying_jobs.sql))
2.  **What skills are required for the top-paying data analyst jobs?** ([`2_top_paying_job_skills.sql`](project_sql/2_top_paying_job_skills.sql))
3.  **What are the most in-demand skills for data analysts?** ([`3_top_demanded_skills.sql`](project_sql/3_top_demanded_skills.sql))
4.  **What are the top skills based on salary?** ([`4_top_paying_skills.sql`](project_sql/4_top_paying_skills.sql))
5.  **What are the most optimal skills to learn?** ([`5_optimal_skills.sql`](project_sql/5_optimal_skills.sql))

## Tools I Used
For my deep dive into the data analyst job market, I harnessed the power of several key tools:
* **SQL:** The backbone of my analysis, allowing me to query the database and unearth critical insights.
* **PostgreSQL:** The chosen database management system, ideal for handling the job posting data.
* **Visual Studio Code:** My go-to for database management and executing SQL queries.
* **Git & GitHub:** Essential for version control and sharing my SQL scripts and analysis.

## The Analysis

### 1. Top Paying Jobs
To identify the highest-paying roles, I filtered for data analyst positions with reported salaries, focusing on remote opportunities.
* **Wide Salary Range:** The top 10 highest-paying remote data analyst roles span from **$184,000 to $650,000**.
* **Top Companies:** Companies like **Meta**, **SmartAsset**, and **AT&T** appear on the top-paying list, showing that tech and telecom giants are leading the market.

### 2. Skills for Top Paying Jobs
To understand what skills these high-paying roles require, I analyzed the job descriptions of the top 10 roles identified in step 1.
* **The "Big 3":** **SQL** (8 mentions), **Python** (7 mentions), and **Tableau** (6 mentions) are the recurring themes.
* **Insight:** Even for the highest-paid roles, foundational technical skills remain the priority.

### 3. Most In-Demand Skills
This analysis identifies the skills most frequently requested in all job postings, regardless of salary.
* **Insight:** **SQL** and **Excel** are the absolute fundamentals, appearing in the majority of job postings.
* **Insight:** **Python** and **Tableau** follow closely, highlighting the importance of programming and visualization for modern analysts.

### 4. Top Skills Based on Salary
Here, I looked at the average salary associated with each skill to find the most lucrative specialized skills.
* **Insight:** **Big Data & ML skills** (like PySpark, Couchbase, and DataRobot) command top salaries, often exceeding $100k average.
* **Insight:** **Cloud computing proficiency** (Elasticsearch, Databricks, GCP) significantly boosts earning potential.

### 5. Most Optimal Skills to Learn
The "optimal" skills are those that are both in high demand (count > 10) and offer high average salaries.
* **Programming:** **Python** and **R** are highly valued (>$100k avg) and in high demand.
* **Cloud:** **Snowflake**, **Azure**, **AWS**, and **BigQuery** offer a great balance of frequent job openings and high pay.

## Data Validation & Limitations
**Error Checking:**
* **Outlier Removal:** To ensure the reliability of the "Top Paying Skills" analysis, I implemented a filter to exclude skills mentioned in fewer than 10 job postings (`HAVING COUNT > 10`). This prevents niche skills with a single high-paying job from skewing the results.
* **Data Consistency:** Only jobs with non-null salary data (`salary_year_avg IS NOT NULL`) were included in salary calculations to ensure statistical accuracy.

## What I Learned
Throughout this adventure, I've turbocharged my SQL toolkit with some serious firepower:
- **🧩 Complex Query Crafting:** Mastered the art of advanced SQL, merging tables like a pro and wielding WITH clauses for ninja-level temp table maneuvers.
- **📊 Data Aggregation:** Got cozy with GROUP BY and turned aggregate functions like COUNT() and AVG() into my data-summarizing sidekicks.
- **💡 Analytical Wizardry:** Leveled up my real-world puzzle-solving skills, turning questions into actionable, insightful SQL queries.

## Closing Thoughts
This project enhanced my SQL skills and provided valuable insights into the data analyst job market. The findings from the analysis serve as a guide to prioritizing skill development and job search efforts. 
