﻿# Automate-The-Job
# AutomateYourJobSearch
- Automating THE ENTIRE job applicaciton proccess on Carleton MySuccess with python, Selenium, and github actions.
- 1. 1_JobMatching.py : This script will scape the MySuccess all jobs Coop board and extract all jobs matching a regex search into the directory "prospectJobs" for later use

variables to customize:
- regexPattern
- MY_USERNAME (.env)
- MY_PASSWORD (.env)
- OPEN_AI_API_KEY (.env)
- coverLetter.txt    (#the cover letter to be customized 

Features:
- Automated login to university portal
- Navigation through co-op job pages
- Extraction of job information based on specified criteria, currently using regex but many alternative methods avalible
- Storage of relevant job information in text files

Dependencies:
  - Python
  - Selenium
  - WebDriver (Chrome)
  - python-dotenv
  - python-docx
  - docx2pdf
    
  

Usage:
  - Set up a virtual environment, activate it,  and install dependencies from requirements.txt.
  - Create a .env file with your login credentials and OPENAI api key.
  - change the regex expression to match jobs you want to target
  - Run the scripts in order 1-4 and thats it!

how to setup venv:
- python -m venv venv               # or python3, depending on your setup
- python -m venv venv               # or python3, depending on your setup
- venv/bin/activate                 # or activate.bat on Windows
- pip install -r requirements.txt 
- #should be good to run now with: python -u filename.py


More requirerements:

Note/Requirements:
  - global variables that need customization are at the top of the file
  - Make sure to customize the criteria(REGEX) in the first script to match your job preferences.
  - Job position name for files is changed to replace invalid characters 
  - global variables that need customization are at the top of the file
  - please enter your login credentionals into a dont env file with approriate varibles before running
  - regexPattern is a gloabal variable that will be used to file matching jobs


Contributing:
Contributions are more that welcome! Feel free to open issues, submit pull requests, or suggest enhancements to make this tool more effective and user-friendly.
  -neccasary improvements:
    - fix jobs page navigation to scrapper each page (currently only does first 100 listing on page 1 of job board)
    - 


