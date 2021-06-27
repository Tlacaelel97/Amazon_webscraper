# Amazon Scraper using Selectorlib 

A simple amazon scraper to extract product details and prices from Amazon.com using Python Requests and Selectorlib. 


There are two simple scrapers in this project. 
1. Amazon Product Page Scraper `amazon.py`
1. Amazon Search Results Page Scraper `searchresults.py`

## Usage

From a terminal 
 
1. Install Requirements `pip3 install -r requirements.txt`

## Scrape Products from Search Results

This scraper only scrapes product from the first page of search results

1. Add Amazon Product URLS to [search_results_urls.txt](search_results_urls.txt)
1. Run `python3 searchresults.py`
1. Get data from [search_results_output.jsonl](search_results_output.jsonl)

## Example Data Format

### Search Results 
Each result would look similar

```json
{
    "title": "New ! Dell Inspiron i3583 15.6\" HD Touch-Screen Laptop - Intel i3-8145U - 8GB DDR4-128GB SSD - Windows 10 - Wireless-AC - Bluetooth - SD Card Reader - HDMI & USB 3.1 -Waves MaxxAudio Pro- Black",
    "url": "/Dell-Inspiron-i3583-Touch-Screen-Laptop/dp/B08173ZTJX/ref=sr_1_3?dchild=1&keywords=laptops&qid=1591584632&sr=8-3",
    "rating": "4.1 out of 5 stars",
    "reviews": "122",
    "price": "$472.00",
    "search_url": "https://www.amazon.com/s?k=laptops"
}
```
Inspired by [ScrapeHero Tutorials](https://www.scrapehero.com/tutorial-how-to-scrape-amazon-product-details-using-python-and-selectorlib/)