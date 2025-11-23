## Web_Scrapping_Project
his project demonstrates end-to-end web scraping using Python, BeautifulSoup, and Requests. The goal is to extract book data from an open, legally scrapable website BooksToScrape.com and prepare it for analysis.

## Project Overview

This project scrapes:

Book Title

Price (cleaned to numeric)

Availability

Rating

Product Page Link

The script also handles:

HTML parsing

Price cleaning (removing currency symbols + corrupted characters)

UTF-8 encoding to prevent garbled symbols

Exporting to CSV

## Technologies Used

Python 3

BeautifulSoup4

Requests

Regular Expressions (re)

CSV module

Jupyter Notebook

## Dataset

After running the script, the final dataset is exported as:

books.csv


Contains 1,000+ book entries from all pages on the website.

## Script Overview
Main modules:
import requests
from bs4 import BeautifulSoup
import csv
import re

Key Features
  UTF-8 decoding for clean text
  Extract book details from multiple pages
  Clean numeric price values
  Export clean tabular data

 ## How to Run
1. Install dependencies
pip install requests beautifulsoup4

2. Run the script
python web_scraping_books.py

3. Output

A new file will appear in the same folder:

books.csv

## Columns in Output
Column	Description
Title	Book title
Price	Numeric price value (clean)
Rating	Star rating
Availability	Stock information
Link	Product URL


## Data Cleaning Notes

Fixed corrupted characters like "Ã‚Â£" → "£"

Removed non-numeric symbols from prices using regex

Stripped whitespace & formatted strings

## Final Summary

This project showcases:

Real-world web scraping

Cleaning messy text data

Exporting structured datasets

Writing reproducible Python scripts
