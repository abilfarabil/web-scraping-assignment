# Web Scraping & GraphQL Data Integration

## Overview
This project demonstrates data integration capabilities by combining web scraping and GraphQL API techniques. It extracts book information from Books to Scrape website and integrates country data from Countries GraphQL API, showcasing essential data engineering skills in data collection and API integration.

## Prerequisites
- Python 3.8+
- Google Colab account
- Required Python libraries:
  - requests==2.28.2
  - beautifulsoup4==4.11.2
  - pandas==1.5.3
  - python-dotenv==0.21.1

## Installation & Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/abilfarabil/web-scraping-assignment.git
   ```
2. Open the Jupyter notebook in Google Colab
3. Run all cells in sequence

## Project Structure
```
project/
├── notebooks/
│   └── Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb
├── data/
│   ├── books_scraped_clean.csv
│   └── countries_data.csv
├── images/
│   ├── 1_Kode_Scraping_Buku.png
│   ├── 2_Kode_Scraping_Buku.png
│   ├── 3_Hasil_Data_Buku.png
│   ├── 4_Kode_GraphQL.png
│   ├── 5_Kode_GraphQL.png
│   └── 6_Hasil_Data_Negara.png
└── README.md
```

## Features
### 1. Web Scraping Implementation
- Automated data extraction from Books to Scrape website
- Handles multiple pages of book listings
- Extracts key book information: Title, Price, and Rating
- Data cleaning and standardization
- Export to structured CSV format

### 2. GraphQL API Integration
- Implementation of GraphQL queries for country data
- Data extraction of country details including code, name, continent, and languages
- Response parsing and data transformation
- Export to structured CSV format

## Implementation Details

### Web Scraping Process
The script performs automated extraction of book data:

![Screenshot of Book Scraping Code](images/1_Kode_Scraping_Buku.png)
![Screenshot of Book Scraping Code](images/2_Kode_Scraping_Buku.png)

Resulting dataset structure:
![Book Data Results](images/3_Hasil_Data_Buku.png)

### GraphQL Implementation
Integration with Countries GraphQL API:

![Screenshot of GraphQL Code](images/4_Kode_GraphQL.png)
![Screenshot of GraphQL Code](images/5_Kode_GraphQL.png)

Final country data structure:
![Country Data Results](images/6_Hasil_Data_Negara.png)

## Output Files
1. `books_scraped_clean.csv`:
   - Contains book information
   - Columns: Title, Price, Rating
   - Clean and standardized format

2. `countries_data.csv`:
   - Contains country information
   - Columns: Code, Name, Continent, Language
   - Structured for easy analysis

## Technologies Used
- Python 3.8+
- BeautifulSoup4 for HTML parsing
- Requests library for HTTP requests
- Pandas for data manipulation
- GraphQL for API queries
- Google Colab as development environment
- Git for version control

## References
- [Books to Scrape](http://books.toscrape.com/)
- [Countries GraphQL API](https://countries.trevorblades.com/)
- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Requests Documentation](https://docs.python-requests.org/en/latest/)
- [GraphQL Documentation](https://graphql.org/learn/)

## Author
Abil Farabil
