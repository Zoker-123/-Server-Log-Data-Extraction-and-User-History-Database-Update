# Server Log Data Extraction and User History Database Update

## Overview
This project processes a server log file (`mbox.txt`) to extract email addresses and their corresponding dates, stores the data in MongoDB and SQLite databases, and performs analytical queries to gain insights. The goal is to create a clean, accurate dataset for historical tracking and analysis.

## Problem Statement
The task is to:
- Extract email addresses and dates from a server log file.
- Transform the data into a standardized format.
- Store the data in MongoDB and SQLite databases.
- Analyze the data with SQL queries to uncover patterns and trends.

## Technologies Used
- **Python**: For data extraction, transformation, and database operations.
- **SQLite**: For relational database storage and querying.
- **MongoDB**: For NoSQL storage of email data.
- **Regex**: For parsing email addresses and dates.
- **python-dateutil**: For flexible date parsing.

## Project Structure
- `email_log_processor.py`: Main Python script with data pipeline and analysis.
- `mbox.txt`: Input log file (not included; provide your own).
- `.gitignore`: Excludes temporary files and database.
- `README.md`: Project documentation.

## Setup Instructions
1. **Prerequisites**:
   - Python 3.x
   - MongoDB running locally (`mongodb://localhost:27017/`)
   - Install dependencies:
     ```bash
     pip install pymongo python-dateutil

## Analytical Queries
The script performs the following analyses:

- List unique email addresses.
- Count emails per day.
- Find first and last email dates per address.
- Count emails per domain.
- Emails per hour of day.
- Emails with multiple entries.
- Top 3 days with most emails.
- Count unique domains.
- Emails active on a specific date.
- Average emails per address.
- Domains active on multiple days.
- Time gap between first and last emails.
- Emails sent in the morning.
- Total number of emails.

## Insights
- **Domain Popularity**: Gmail dominates email activity, followed by Yahoo.
- **Temporal Patterns**: Most emails are sent in early morning hours (e.g., 00:00–02:00).
- **User Activity**: Some users send emails across multiple days, indicating consistent engagement.
