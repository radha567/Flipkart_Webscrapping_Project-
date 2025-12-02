# Flipkart_Webscrapping_Project-
📌 Overview

This project extracts product details such as name, price, and rating from Flipkart using Python, BeautifulSoup, and Requests.
The scraped data is cleaned and stored in a CSV file for further analysis, making it useful for price comparison, trend analysis, and dataset creation.

🚀 Features

Scrapes multiple product attributes

Extracts Product Name, Price, Rating

Stores data in a structured CSV file

Simple and reusable Python script

Useful for data analysis and machine learning

🛠️ Tech Stack

Python

BeautifulSoup (bs4)

Requests

Pandas

📂 Project Structure
├── flipkart_scraper.ipynb
├── data.csv
├── README.md

📜 How It Works

Send a GET request to the Flipkart search page

Parse HTML using BeautifulSoup

Extract product details using class selectors

Store the scraped data into lists

Convert the data into a Pandas DataFrame

Export to CSV

🧩 Sample Code Snippet
product = soup.find_all("a", class_="pIpigb")
for i in product:
    name.append(i.get_text(strip=True))

price_tag = soup.find_all("div", class_="hZ3P6w")
for i in price_tag:
    price.append(i.get_text(strip=True))

rating_tag = soup.find_all("div", class_="a7saXW WDsrYC")
for i in rating_tag:
    rating.append(i.get_text(strip=True))

📊 Output

✔ Clean CSV file containing

Product Name

Price

Rating

📈 Use Cases

Price monitoring

Product comparison

Dataset preparation

E-commerce analytics

⚠️ Disclaimer

This project is for educational purposes only.
Scraping e-commerce websites may violate their Terms of Service.
Use responsibly.
