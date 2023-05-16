# install django

python -m pip install django

# start new project

django-admin startproject jtracker

# run project

cd jtracker/jtracker
python manage.py runserver

# this will show a url the development sever

# add site

cd jtracker (directory with manage.py)
python manage.py startapp jsite

# Add website to the INSTALLED_APPS in settings.py

# URL path in urls.py
python manage.py runserver
http://127.0.0.1:8000/welcome.html

# How to Use Python Requests with REST APIs
# https://www.nylas.com/blog/use-python-requests-module-rest-apis/
pip install requests



 
https://stackoverflow.com/questions/44979299/extracting-asx-data-using-pandas 


Individual stock  
https://www.asx.com.au/asx/1/share/WOW

Individual stock details
https://www.asx.com.au/asx/1/company/WOW?fields=primary_share,latest_annual_reports,last_dividend,primary_share.indices

Individual stock daily price
https://www.asx.com.au/asx/1/share/WOW/prices?interval=daily&count=255 
https://www.asx.com.au/asx/1/share/WOW/prices?interval=daily&count=40 

Individaul stock dividends
https://www.asx.com.au/asx/1/company/WOW/dividends
https://www.asx.com.au/asx/1/company/WOW/dividends/history?years=5

Individual stock announcements
https://www.asx.com.au/asx/1/company/WOW/announcements?count=20&market_sensitive=true

Individual stock key people
https://www.asx.com.au/asx/1/company/WOW/people

ASX listed companies in CSV file
https://www.asx.com.au/asx/research/ASXListedCompanies.csv 

================================================================

# Endpoint providing CSV of listed companies and their tickers
asx_companies_csv: https://www.asx.com.au/asx/research/ASXListedCompanies.csv 

# Endpoint providing XLS spreadsheet of all listed securities and their tickers
asx_securities_tsv: https://www.asx.com.au/programs/ISIN.xls 
    # NOTE the extension is xls but the file is actual tab separated

# Endpoint to pull individual companies data
asx_company_json: https://www.asx.com.au/asx/1/company/%s?fields=primary_share,latest_annual_reports,last_dividend,primary_share.indices
    # %s = ticker

# Endpoint to pull individual securities data
asx_single_json: https://www.asx.com.au/asx/1/share/%s 
  # %s = ticker
  # OLD; http://data.asx.com.au/data/1/share/%s

# Endpoint to pull announcements
asx_announcements_json: https://www.asx.com.au/asx/1/company/%s/announcements?count=20&market_sensitive=true
    # %s = ticker

# Endpoint for pulling historical ASX stock prices
floatau_historical_csv: http://float.com.au/download/%s.csv?format=stockeasy  # %s = ticker





