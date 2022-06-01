# Web-Scraping-Chocolate-Dataset
## Problem 
I wanted to do some analysis on chocolate production countries from https://flavorsofcacao.com/chocolate_database.html but couldn't download the dataset to do some local SQL-kind-of analysis.

## Dependencies
- [Python](https://www.python.org/downloads/)
- [Python Data Analysis Library (Pandas) ](https://pandas.pydata.org/pandas-docs/stable/install.html#installing-from-pypi)
- [Python Web Scraping Library (BeautifulSoup4) ](https://pypi.org/project/beautifulsoup4/)
- [Python HTTP Library (Requests) ](https://pypi.org/project/requests/)
- [Python Parser Library (Requests) ](https://pypi.org/project/csv/)

## Solution 
### Web Scraping
I had to do some web scraping of my own in order to attain that dataset. I thought it would be a simple import of request and beautifulsoup libraries on python type of process but no as that website is using Spry Framework in order to export the dataset. I went ahead and used Brave developer tool, opened up insept for that page and reloaded while keeping a watch from where this AJAX thing is coming from. After a long hour of understanding what's happening, I FOUND IT in another html page and linking you to this http://flavorsofcacao.com/database_w_REF.html

### Cleaning 
After finally downloading that chocolate dataset as csv, I noticed there are 87 cells with missing values in Ingredint column and moving that dataset into analysis phase would have made it a bit hard for me so I improvised and decided to replace those NaN cells with empty spaces " " as a value so it would sustain its original shape but with no missing/null value when it is being called.
