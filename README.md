# Web Scraping LinkedIn Jobs: Data Analyst Positions in Egypt (as of 8/4/2025)

This project demonstrates how to scrape **Data Analyst** job listings from **LinkedIn** for positions in **Egypt**. The focus is on extracting job details, including job titles, company names, locations, insights, responsibilities, qualifications, and benefits.

## Project Overview
- **Objective**: Scrape LinkedIn job listings for Data Analyst roles in Egypt, as of **April 9, 2025**.
- **Output**: CSV files containing job details, insights, and job-specific sections.

## Files Included

### 1. **linkedin_job_containers_working(150job).py**
   - **Purpose**: This script scrapes the first 150 **Data Analyst** job listings from LinkedIn in Egypt. It collects basic information such as:
     - Job title  
     - Company name  
     - Job location  
     - Easy apply option status  
     - Job link
   - The results are saved in the CSV file: **linkedin_job_containers_working(150job).csv**.
   
   - **How It Works**:
     - The script scrapes 6 pages of LinkedIn job listings, extracting job titles, company names, locations, and easy apply status.
     - The results are saved into a CSV file for further analysis.

   - **Challenges**:  
     - LinkedIn’s high security and its detection mechanisms against **Selenium** made this project challenging. LinkedIn is highly sensitive to bot activity, so the code must carefully simulate human actions to avoid detection.
   
### 2. **job_details_of_1st_page_working.py**
   - **Purpose**: This script enhances the first version by scraping detailed job data for each job listing. It collects:
     - Job title  
     - Company name  
     - Job location  
     - Easy apply option status  
     - Job link  
     - Insights (Insight 1, Insight 2, Insight 3)  
     - Responsibilities  
     - Qualifications  
     - Benefits  
     - Job summary
   - The results are saved in the CSV file: **job_details_of_1st_page_working.csv**.

   - **How It Works**:
     - After gathering the job URLs, the script goes through each job's detailed page and scrapes additional data, such as responsibilities, qualifications, and job summary.
     - It also collects insights about the job that are available in the job posting.

   - **Challenges**:  
     - LinkedIn’s high security and its detection mechanisms against **Selenium** required extra caution in scraping. The code needed to handle dynamic page content, scrolling to load more jobs, and simulating user behavior to avoid being flagged as a bot.

## Requirements

To run this project, you'll need:
- **Python 3.x**
- **Selenium**: A Python library used for automating web browsers.
   - Install via `pip install selenium`.
- **BeautifulSoup**: For parsing HTML and extracting job details.
   - Install via `pip install beautifulsoup4`.
- **ChromeDriver**: Required for Selenium to control the Chrome browser.

## How to Use

1. Clone or download the repository to your local machine.
2. Install the required dependencies by running:
   ```bash
   pip install selenium beautifulsoup4
