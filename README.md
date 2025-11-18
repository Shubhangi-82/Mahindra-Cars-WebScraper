🚗 Mahindra Cars Web Scraping Project
**Python | Selenium | BeautifulSoup | Pandas**

This project was completed as part of my internship at **Evoastra Ventures**.
The objective was to **scrape detailed data of used Mahindra cars** from *Cars24* across multiple locations (Mumbai, Delhi, Hyderabad), process it, clean it, and store it in a structured CSV format for analysis.
 📌 **Project Overview**

We automated data extraction for Mahindra cars, collecting:

* Car Name
* Price
* Year
* Fuel Type
* Transmission
* KM Driven
* Location
* Number of Owners
* Car Rating
* URL for each listing

The data was scraped for:
✔ **Mumbai**
✔ **Delhi**
✔ **Hyderabad**

The final dataset was exported as separate CSV files for each city.

🛠️ **Tools & Libraries**

* **Python**
* **Selenium WebDriver**
* **BeautifulSoup**
* **Pandas**
* **ChromeDriver**
* **Time / OS modules**


🔍 **Key Challenges & Solutions**

**1️⃣ Infinite Scrolling**

Cars24 loads only 20 cars at a time.
✔ *Solution:* Implemented Selenium auto-scrolling until no new cars appeared.

**2️⃣ Missing Data (None values)**

Some car details like “Number of Owners” were missing.
✔ *Solution:* Added validation and replaced missing values with `"Not Mentioned"`.

**3️⃣ Duplicate Entries**

Scrolling sometimes repeated the same car.
✔ *Solution:* Used **pandas.drop_duplicates()** to remove duplicate rows.

**4️⃣ Deprecation Warning**

BeautifulSoup’s `text=` argument was outdated.
✔ *Solution:* Updated to `string=` to fix warnings.


🚀 **How to Run**

1. Install dependencies

pip install selenium beautifulsoup4 pandas

2. Download **ChromeDriver** matching your browser version.

3. Run the script

python mahindra_scraper.py

4. CSV files will be auto-saved in your directory.


 📊 **Output Sample**

| Car Name        | Price     | Year | Fuel   | KM Driven | Owners    | Location |
| --------------- | --------- | ---- | ------ | --------- | --------- | -------- |
| Mahindra XUV500 | ₹7,80,000 | 2017 | Diesel | 58,000 km | 1st Owner | Mumbai   |


⭐ **If you like this project, consider giving it a star!**

It motivates me to share more work on data analysis & automation.



