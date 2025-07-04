# Green Consultant - SDG Module Analyzer

A Python script designed to analyze university module webpages and identify connections with the United Nations Sustainable Development Goals (SDGs) by searching for relevant keywords in the module content.

---

## Features

- ✅ Scrapes module URLs from university course pages  
- ✅ Extracts and cleans visible text from each module page  
- ✅ Analyzes content against 17 SDG keyword lists  
- ✅ Generates a comprehensive CSV report summarizing SDG keyword matches  
- ✅ Runs Chrome in headless mode for efficient and silent processing  

---

## Requirements

- Python 3.7 or higher  
- Google Chrome browser installed  
- [Selenium](https://selenium-python.readthedocs.io/) Python package  
- ChromeDriver (compatible with your installed Chrome version)  

---

## Installation

1. Install Selenium via pip:

   ```bash
   pip install selenium


Usage
Configure the script variables:

filepath — Path where the results CSV will be saved.

url — The target university course modules page URL to scrape.

Run the script:

The script will:

Scrape all module URLs from the given course page

Extract visible text content from each module page

Search the content for keywords linked to the 17 SDGs

Output a CSV file listing each module, URL, and the matched SDG keywords

Example Output Format
Module Code	URL	Matched SDG Keywords
CLA1001	https://.../CLA1001	SDG 4: pedagogy; SDG 5: gender identity

Default Target URL
The script is pre-configured to analyze modules from the University of Exeter's Classics program:

ruby
Copy
Edit
https://www.exeter.ac.uk/study/studyinformation/modules/?prog=classics&year=2025/6
Notes
Chrome runs in headless mode by default for better performance and less resource usage.

You may need to adjust time.sleep() durations within the script depending on your network speed to ensure all content loads properly.

The SDG keyword lists are customizable within the sdg_keywords dictionary in the script to better fit your analysis needs.
