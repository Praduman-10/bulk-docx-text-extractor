# SDG Module Analyzer

A Python tool that analyzes university course modules for Sustainable Development Goal (SDG) relevance by scanning webpage content for SDG-related keywords.

## Features

- 🕸️ Web scraping of module pages  
- 🔍 Keyword analysis against all 17 SDGs  
- 📊 CSV report generation  
- 🚀 Headless browser operation  
- ⚙️ Customizable keyword lists  

## Usage

1. Configure the target URL and output file path in the script:

```python
url = "https://www.exeter.ac.uk/study/studyinformation/modules/?prog=classics&year=2025/6"
filepath = "results.csv"  # Output CSV file path
```

## Customization

Customize SDG keywords as needed:

```python
sdg_keywords = {
    "SDG 1": ["poverty", "economic justice", "welfare"],
    "SDG 2": ["food justice", "sustainable agriculture"],
    "SDG 3": ["public health", "wellbeing"],
    "SDG 4": ["education", "inclusive learning"],
    "SDG 5": ["gender equality", "feminism"],
    # ... continue for all 17 SDGs ...
}


### Setup

```bash
# Install required package
pip install selenium

# Download ChromeDriver (match your Chrome version)
# https://chromedriver.chromium.org/downloads

