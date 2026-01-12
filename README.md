# Web Scraping Project: Asian Countries by Area

## Overview

This project demonstrates **web scraping** and **data extraction** from Wikipedia using Python.
The goal was to scrape a table listing **Asian countries by area** and convert it into a **clean, structured Pandas DataFrame** ready for analysis.

---

## Tools & Libraries

* **Python 3.x**
* **Requests** – HTTP requests
* **BeautifulSoup (bs4)** – HTML parsing
* **Pandas** – Data manipulation

---

## Approach

1. **Fetch Page Content**

   * Used `requests.Session()` with a **descriptive User-Agent** to comply with Wikimedia’s policies.

2. **Parse HTML**

   * Used **BeautifulSoup** to locate the target table in the page.

3. **Extract Table Rows**

   * Iterated through `<tr>` elements and `<th>/<td>` cells.
   * Cleaned text using `.get_text(strip=True)` to remove extra whitespace.

4. **Convert to Pandas DataFrame**

   * Used `pd.read_html()` to directly parse the HTML table into a DataFrame.
   * The resulting table is ready for **analysis, visualization, or export**.

---

## Outcome

* Successfully scraped and **structured data** into a Pandas DataFrame.
* Demonstrated **web scraping best practices**:

  * Custom User-Agent headers
  * HTML parsing
  * Data cleaning and formatting
* Ready for **analysis, visualization, or export to CSV/Excel**.

