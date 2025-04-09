Web Scraping LinkedIn Jobs: Data Analyst Positions in Egypt (as of 9/4/2025)

This project involves web scraping LinkedIn job listings specifically for Data Analyst positions in Egypt. The scraping is done for job listings available on April 9, 2025.

Files:
linkedin_data_analyst_in_egypt_jobs.py:
This script scrapes all available pages for Data Analyst job listings in Egypt on LinkedIn (at the specified date). It retrieves data from 6 pages and collects the following information for each job:

Job title

Company name

Job location

Easy apply option status

The results are saved in a CSV file named linkedin_data_analyst_in_egypt_jobs.csv.

linkedin_data_analyst_in_egypt_jobs_v2.py:
In this updated version, the script loops through each individual job and extracts additional job-specific sections, including:

Insight 1, Insight 2, Insight 3

Responsibilities

Qualifications

Benefits

Job summary

If any of these sections are missing for a job, the code handles the exception and populates the missing fields with "NA" instead of throwing an error.

Key Features:
The script is designed to be adaptable to any job search in any country with minimal code adjustments.

The output is stored in a structured CSV format for easy analysis.

This project demonstrates how to scrape LinkedIn job listings and handle missing data effectively, making it an excellent foundation for data collection tasks in job market analysis.

How to Use:
To apply this code to other job types or countries, simply modify the search query and adjust any country-specific settings in the code.
