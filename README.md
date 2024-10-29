# Amazon Product Information Scraper Python Project
**Overview**

The **Amazon Product Information Scraper** is a Python-based tool designed to extract essential details from product pages on Amazon. Utilizing the Beautiful Soup library for web scraping, this project allows users to obtain product titles, prices, ratings, review counts, and availability status efficiently. Whether conducting market research, comparing products, or collecting data for analysis, this tool provides a streamlined approach to accessing valuable information from one of the world's largest e-commerce platforms.

**Features**

* **Product Title Extraction:** Captures the product name for easy identification.
  
* **Price Retrieval:** Fetches the current price of the product, formatted for clarity.
  
* **Rating and Reviews:** Gathers product ratings and total review counts to gauge customer feedback.
  
* **Availability Status:** Checks and records whether the product is in stock or not.
  
* **CSV Output:** Saves the collected data in a CSV file for easy analysis and manipulation.

**Requirements**

To run this project, the following must be installed:

* Python 3.x
* Beautiful Soup 4
* Requests library
  
The necessary libraries can be installed using pip:

      pip install beautifulsoup4 requests

**Usage**

1) Clone the repository or download the script.
2) Ensure that the required libraries are installed.
3) Open the script and modify the URL in the **main** function to the desired Amazon product page.
4) Run the script:

      python amazon_scraper.py

5) The scraped information will be saved in a file named **out.csv**.

**Code Explanation**

The core of the scraping process is encapsulated within the **main** function. Here is a brief overview of how it works:

* **HTTP Request:** The script initiates a request to the specified Amazon product URL with a user-agent header to mimic a browser.

* **HTML Parsing:** It parses the HTML content using Beautiful Soup to extract the necessary information.

* **Data Extraction:** The script searches for specific HTML elements to retrieve the product title, price, rating, review count, and availability.

* **Error Handling:** It includes error handling to manage missing data gracefully, ensuring robust performance.

* **CSV Writing:** Finally, the collected data is appended to a CSV file for further use.

**Example**

Here's an example of how to call the scraper function:

      if __name__ == '__main__':
          main("https://www.amazon.com/Dremel-Education-Accessories-Professional-Development/dp/B07KZ8XNDT")

**Conclusion**

The Amazon Product Information Scraper demonstrates the power of Python for web scraping, enabling efficient automation of data collection from Amazon product pages. With its user-friendly interface and robust functionality, this project serves as a valuable tool for anyone looking to analyze product data efficiently.






