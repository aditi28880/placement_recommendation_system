# Python based placement recommendation system
A Flask-powered placement recommendation system developed as part of my BSc Computer Science final year project. This system efficiently bridges the gap between job seekers and recruiters by providing personalized job recommendations and candidate matching based on skills, experience, and job roles.
# Project Overview
This project is a web-based application built using Python and Flask. It leverages machine learning algorithms to generate job recommendations and facilitate recruiter-candidate interactions.

## Job Seekers can:
-Register, log in, and update their profile with skills, experience, and job preferences.
 Receive top job recommendations tailored to their profile.

## Recruiters can:
-Log in using company credentials.
Access a list of recommended candidates for specific job postings.

# Technology used
Frontend: HTML, CSS, JavaScript

Backend: Python (Flask framework)

Database: PostgreSQL

Machine Learning: Pandas, NumPy, Scikit-learn for job recommendation logic, TF-IDF Vectorization

Operating System: Linux

# Project Structure
app.py-Main Flask application handling user authentication, job recommendations, and recruiter functionalities.

jobs1.py-Implements the job recommendation algorithm using data science libraries.

jobs_info.csv- The Dataset containing job details, including job ID, salary, experience, skills, industry, and title.

companies_table.txt-SQL script for creating and populating the companies table with sample recruiters' credentials.

templates-HTML templates for the web interface.

# Setup & Execution Guide
## 1) Environment Setup  
Ensure Python is installed and install the required dependencies:  
```
pip install flask psycopg2-binary pandas scikit-learn numpy werkzeug
```
## 2) Database Configuration
1.Install and configure PostgreSQL. 

2.Create a new database:
```
CREATE DATABASE placement;
```
3.Set up the companies table:

-Open companies_table.txt and copy the provided SQL statements.

-Execute these statements in your PostgreSQL client (pgAdmin, command line, or any SQL interface).

-This will create and populate the companies table with sample recruiter credentials.



## 3)Running the Application
Navigate to the project directory and start the Flask application:
```
python3 app.py
```

## 4)Using the Application
1)Open http://localhost:5000 in a browser.

### -> For Job Seekers:
1. **Sign up** or **log in** to your account.  
2. Click **"Recommend jobs for me"** to get AI-powered job recommendations.  
   - Top **10 job recommendations** based on your **experience, skills, and job title**.  
   - Recommendations are stored in the **recommendations table**.  

---

### -> For Recruiters:
1. **Log in** using company credentials (stored in the **companies table**).  
2. **View recommended candidates** or **browse existing job listings**.  
3. To **log out**, use the **navigation bar** and return to the homepage.  

---










