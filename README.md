SecureLog Analyzer

Project Overview

The SecureLog Analyzer is a Python-based tool designed to parse, analyze, and visualize security-related log entries. It helps in identifying potential threats such as brute-force attacks and unauthorized access attempts through an interactive dashboard. This updated version includes a more professional user interface and the ability to upload custom log files for analysis.

Project Structure

Plain Text


securelog-analyzer/
│
├── logs/
│ └── sample.log
│
├── utils.py
├── detector.py
├── dashboard.py
├── requirements.txt
└── README.md



•
logs/sample.log: Contains a larger and more diverse set of sample log entries for analysis.

•
utils.py: Provides utility functions for parsing and filtering log data.

•
detector.py: Implements logic for detecting security threats like brute-force attacks and other critical threats, now capable of handling dynamic log data sources.

•
dashboard.py: Creates an interactive web dashboard using Streamlit, featuring a professional UI, log level distribution, threat summaries, and a log file upload feature.

•
requirements.txt: Lists all the Python dependencies required to run the project.

•
README.md: This file, providing an overview and instructions.

Features

•
Enhanced Log Parsing: Efficiently parses log entries from a specified file or uploaded data.

•
Advanced Threat Detection: Identifies common security threats such as:

•
Brute-force attacks (repeated failed login attempts from the same IP).

•
Unauthorized access attempts.

•
SQL Injection attempts.

•
Malicious file uploads.



•
Professional Interactive Dashboard: A user-friendly Streamlit dashboard for:

•
Log File Upload: Easily upload your own .log or .txt files for analysis.

•
Viewing comprehensive log summaries.

•
Visualizing log level distribution with interactive charts.

•
Displaying detailed detected threats.

•
Filtering log entries by level.

•
Downloading filtered log entries as CSV.



Setup and Installation

1.
Clone the repository (or create the files manually as provided):

Bash


git clone <repository_url>
cd securelog-analyzer





2.
Install dependencies:

Bash


pip install -r requirements.txt





Usage

1.
Run the Streamlit dashboard:

Bash


streamlit run dashboard.py





2.
Open your web browser and navigate to the URL provided by Streamlit (usually http://localhost:8501 ).

3.
Upload Your Log File: Use the "Upload a log file" section in the sidebar to upload your .log or .txt file. The dashboard will automatically update with the analysis of your uploaded logs.

How to Extend

•
Add new log formats: Modify utils.py to include new parsing logic.

•
Implement new detection rules: Extend detector.py with more sophisticated threat detection algorithms.

•
Enhance dashboard: Add more visualizations, filtering options, or advanced features in dashboard.py.

License

This project is open-source and available under the MIT License. See the LICENSE file for more details. (Note: LICENSE file is not part of this project delivery, but can be added if needed.)

