Task 1: Web Scraping - Goodreads Book List
This project is part of my internship with CodeAlpha. The goal of this task was to practice web scraping by extracting book titles and authors from a public Goodreads list.

Objective
To build a Python script that scrapes data from the Goodreads website and exports it as a structured CSV file for future analysis.

Tools and Libraries Used
Python

requests

BeautifulSoup (bs4)

pandas

time (for polite scraping delays)

How It Works
The script sends a GET request to a Goodreads list page using a browser-like user agent header.

HTML content is parsed using BeautifulSoup.

Book titles and their respective authors are extracted using CSS selectors.

A delay is introduced after each request to avoid overloading the server.

The final data is saved to a goodreads_books.csv file.

Example URL Scraped
https://www.goodreads.com/list/show/1 – "Best Books Ever"

Output
A CSV file containing the following columns:

Title

Author

Usage
Simply run the script using any Python environment. Make sure you have installed all dependencies (bs4, pandas, requests).

bash
Copy
Edit
pip install beautifulsoup4 pandas requests
Then run:

bash
Copy
Edit
python script_name.py
Notes
This script scrapes only the first page of the Goodreads list.

For ethical scraping, a delay of 2 seconds is added between requests.

Data is stored in goodreads_books.csv.