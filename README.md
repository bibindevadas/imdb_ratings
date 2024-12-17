# IMDB Top Rated Movies Web Scraper

This project is a simple **Python web scraping script** that extracts the top-rated movies from the IMDB website: [IMDB Top 250 Movies](https://www.imdb.com/chart/top/). The extracted data includes:

- Movie Rank  
- Movie Name  
- Year of Release  
- IMDB Rating  

The data is saved in an **Excel file** (`IMDB Movie Ratings.xlsx`) using the OpenPyXL library.

---

## **Table of Contents**
1. [Features](#features)
2. [Requirements](#requirements)
3. [Setup and Installation](#setup-and-installation)
4. [Code Walkthrough](#code-walkthrough)
5. [How to Run](#how-to-run)
6. [Output Example](#output-example)
7. [License](#license)

---

## **Features**

- Scrapes IMDB's Top 250 Movies list.  
- Extracts movie rank, title, year of release, and IMDB rating.  
- Saves the data into a structured Excel file for easy analysis.  

---

## **Requirements**

Ensure you have the following installed:

- Python 3.x  
- Required libraries:
  - `beautifulsoup4`  
  - `requests`  
  - `openpyxl`  

---

## **Setup and Installation**

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/your-username/imdb-webscraper.git
    cd imdb-webscraper
    ```

2. Install the required Python libraries:

    ```bash
    pip install beautifulsoup4 requests openpyxl
    ```

3. Ensure you have an active internet connection to access the IMDB page.

---

## **Code Walkthrough**

Here's a quick breakdown of the script:

- **Imports**: The script uses `BeautifulSoup` for parsing HTML, `requests` to fetch web data, and `openpyxl` to handle Excel files.  
- **Workbook Setup**: Creates an Excel file (`IMDB Movie Ratings.xlsx`) with appropriate column headers.  
- **Web Scraping**:  
  - Fetches the IMDB Top 250 Movies page.  
  - Parses the movie table and extracts rank, title, year, and rating.  
- **Data Storage**: Appends extracted data to the Excel file.  
- **Error Handling**: Handles any request or scraping errors.  

---

## **How to Run**

1. Open a terminal or command prompt.  
2. Run the Python script:

    ```bash
    python imdb_scraper.py
    ```

3. After running, the output Excel file `IMDB Movie Ratings.xlsx` will be saved in your project directory.  

---

## **Output Example**

Here is an example of the Excel file output:

| Movie Rank | Movie Name                | Year of Release | IMDB Rating |
|------------|---------------------------|-----------------|-------------|
| 1          | The Shawshank Redemption  | 1994            | 9.3         |
| 2          | The Godfather             | 1972            | 9.2         |
| 3          | The Dark Knight           | 2008            | 9.0         |


---

## **Acknowledgments**

- **IMDB**: The movie data is extracted from [IMDB's Top 250 Movies](https://www.imdb.com/chart/top/).  
- **BeautifulSoup**: For making HTML parsing seamless.  

