# Web Scraping: Largest Companies by Market Cap

## Project Description

This project uses **Selenium** to scrape data from [companiesmarketcap.com](https://companiesmarketcap.com/), a website that updates the list of the world's largest companies by market capitalization.

The goal is to collect useful information about each company: name, stock symbol (ticker), market cap, stock price, and country.

## Project Goals

- Get the most recent list of top global companies
- Extract important data: name, ticker, market cap, price, country
- Bypass bot protection to collect data successfully

## Tools Used

| Tool              | Purpose                                 |
|-------------------|------------------------------------------|
| Python            | Programming language                     |
| Selenium          | To scrape websites with JavaScript       |
| Pandas            | To clean and organize the data           |
| ChromeDriver      | To control the Chrome browser via Selenium |

## Why Selenium?

This website uses JavaScript to load the data. That means tools like `BeautifulSoup` won't work because they only see the basic HTML (not the dynamic content).

Selenium solves this because it:

- Opens a real browser window
- Waits for the page to fully load
- Acts like a real user
- Helps avoid simple anti-bot systems

## Output Example

### Website screenshot:

![Website Screenshot](./screenshots/website.png)

### Sample scraped data:

```
       name company_code market_cap    price country
0     Apple         AAPL    $3.369 T  $222.91     USA
1    NVIDIA         NVDA    $3.320 T  $135.37     USA
2  Microsoft         MSFT    $3.051 T  $410.37     USA
```

## How This Can Be Used

- Track changes in company market cap over time
- Analyze which countries have the most top companies
- Create dashboards using tools like Tableau or Power BI
- Combine with other finance data sources for deeper insights


